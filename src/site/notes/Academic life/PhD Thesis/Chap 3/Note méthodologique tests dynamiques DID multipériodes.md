---
{"dg-publish":true,"permalink":"/academic-life/ph-d-thesis/chap-3/note-methodologique-tests-dynamiques-did-multiperiodes/","hide":true}
---


## 1. Contexte

Nous utilisons la commande **`did_multiplegt_dyn`** (Stata) pour estimer les effets dynamiques de l’adoption d’un NAP (National Adaptation Plan) sur les engagements d’aide (`commitments`).  
L’approche repose sur un **DID multi-groupes avec adoption échelonnée**, et produit :
- des **effets dynamiques post-traitement** (Effets 1, 2, …) ;
- des **placebos** (leads) permettant de tester l’hypothèse de tendances parallèles et de non-anticipation.
---
## 2. Options principales

- **`effects(#)`** : nombre de périodes post-traitement incluses.  
    Exemple : `effects(5)` → estime l’effet jusqu’à 5 ans après l’adoption.
- **`placebo(#)`** : nombre de périodes pré-traitement (leads).  
    Exemple : `placebo(3)` → estime des « pseudo-effets » 3 ans avant adoption.  
    ⚠️ **Règle** : le nombre de placebos ne peut pas dépasser le nombre d’effets.
- **`same_switchers`** : impose que tous les effets (post-traitement) soient calculés sur **le même échantillon de pays**, à savoir ceux qui disposent de suffisamment de données avant et après adoption.  
    → Avantage : comparabilité parfaite entre les effets.  
    → Inconvénient : réduit fortement le nombre de switchers (ex. de 38 à 12).
- **`same_switchers_pl`** (non utilisé ici) : applique la même logique aux placebos.
- **`normalized` / `normalized_weights`** : recentre les coefficients de l’étude d’événement par rapport à l’année d’adoption et corrige les déséquilibres liés aux poids.
- **`controls()`** : ajoute des variables de contrôle (ex. PIB, indicateurs institutionnels).
- **`weight(population)`** : pondération par la population du pays récipiendaire.
---
## 3. Ce que montrent nos différents essais

### (a) Horizons courts (effects(2–3))

- Exemple : `effects(2) placebo(2)` → plus de switchers (28).
- Résultats : effets positifs et significatifs la 1ère année après adoption (+160 à +196), puis effet qui s’atténue ou devient nul.
- Placebos : non significatifs (p-value ~0.18 à 0.45) → pas d’évidence forte de violation de tendance parallèle.  
    👉 Bonne crédibilité causale, mais horizon court (on ne voit pas le moyen terme).
![Pasted image 20250902163121.png](/img/user/Pasted%20image%2020250902163121.png)
![Pasted image 20250902163159.png](/img/user/Pasted%20image%2020250902163159.png)
### (b) Horizons moyens (effects(4))
- ~16 switchers.
- Résultats : effet positif fort la 1ère année (+196), nul les années 2-3, puis rebond positif en année 4 (+75, significatif).
- Placebos : toujours non significatifs (p ≈ 0.48).  
    👉 Résultats cohérents, mais échantillon réduit → moins de puissance.
![Pasted image 20250902163258.png](/img/user/Pasted%20image%2020250902163258.png)
### (c) Horizons longs (effects(5))
- Avec `same_switchers`: seulement 12 switchers.
![Pasted image 20250902163325.png](/img/user/Pasted%20image%2020250902163325.png)
- Résultats : effets très volatils (positifs puis négatifs, puis rebond). Significativité fragile.
- Placebos : non significatifs mais large incertitude (peu d’obs.).  
    👉 Interprétation délicate, car l’échantillon devient très restreint.
- Sans `same_switchers`: plus de switchers (38 la 1ère année), mais composition change d’une période à l’autre. Les effets deviennent plus instables, et les placebos montrent davantage de déviation (parfois significatives).  
    👉 Moins crédible d’un point de vue identification.
![Pasted image 20250902163353.png](/img/user/Pasted%20image%2020250902163353.png)
---

## 4. Enseignements

1. **Choix d’horizon** :
    - La majorité des pays n’ont que 2–3 ans post-adoption dans le panel → demander `effects(5–6)` réduit énormément le nombre de switchers.
    - L’option réaliste est donc **`effects(3)` comme specification principale**.
2. **Parallel trends** :
    - Avec horizons courts/moyens, les placebos sont non significatifs → hypothèse de tendances parallèles raisonnablement soutenue.
    - Sans `same_switchers`, les tests de placebos sont plus souvent rejetés → moins crédible.
3. **Interprétation** :
    - L’adoption d’un NAP est associée à une **hausse significative des engagements d’aide la 1ère année** (≈ +160 à +200).
    - Les effets s’estompent ensuite, voire deviennent négatifs ou nuls, avant un éventuel rebond à moyen terme (selon spécification).
    - L’effet total cumulé est positif, mais l’amplitude dépend fortement de l’échantillon et des covariables incluses.

---

## 5. Recommandations pour la rédaction

- **Résultats principaux** : présenter la spécification `same_switchers effects(3) placebo(3)` comme estimation de référence.
- **Robustesses** :
    - montrer horizons plus longs (`effects(4–5)`) en annexe ;
    - comparer avec et sans `same_switchers`.
- **Graphiques** : inclure plots d’étude d’événement (avec barres de confiance) pour visualiser les dynamiques.
- **Discussion** : souligner que la crédibilité causale repose surtout sur horizons courts/moyens (où les placebos ne sont pas significatifs et l’échantillon est encore substantiel).
- regarder aide / aide total 

---
## 6. Résumé regressions
### (a) Effets dynamiques estimés

| Spécification                                   | Switchers | Effet_1   | Effet_2  | Effet_3  | Effet_4   | Effet_5   | Test joint effets (p) |
| ----------------------------------------------- | --------- | --------- | -------- | -------- | --------- | --------- | --------------------- |
| **effects(2), placebo(2), same_switchers**      | 28        | **+162*** | +58 (ns) | –        | –         | –         | 0.001                 |
| **effects(3), placebo(3), same_switchers**      | 18        | **+196*** | +18 (ns) | -14 (ns) | –         | –         | 0.003                 |
| **effects(4), placebo(3), same_switchers**      | 16        | **+196*** | +31 (ns) | -13 (ns) | **+75***  | –         | 0.000                 |
| **effects(5), placebo(3), same_switchers**      | 12        | **+86***  | -49 (ns) | -47 (ns) | **+51**   | +64 (ns)  | 0.002                 |
| **effects(5), placebo(3), sans same_switchers** | 38→12     | **+183*** | +97 (ns) | -41 (ns) | **+326*** | +308 (ns) | 0.00001               |

> Notes : (ns) = non significatif ; * = significatif 5% ; ** = 1% ; *** = 0.1%.  
> Les switchers diminuent fortement quand on impose `same_switchers` car il faut ≥3 ans avant ET ≥N années après adoption pour être inclus.

---

### (b) Tests de placebo (tendances parallèles)

|Spécification|Placebo_1|Placebo_2|Placebo_3|Test joint placebos (p)|
|---|---|---|---|---|
|**effects(2), same_switchers**|+113 (ns)|+34 (ns)|–|0.18|
|**effects(3), same_switchers**|+79 (ns)|+93 (ns)|+101 (ns)|0.45|
|**effects(4), same_switchers**|+59 (ns)|+93 (ns)|+61 (ns)|0.48|
|**effects(5), same_switchers**|+122 (ns)|+43 (ns)|+33 (ns)|0.48|
|**effects(5), sans same_switchers**|+66 (ns)|+52 (ns)|+288 (ns, large CI)|0.30|

> Observation : avec `same_switchers`, les placebos ne sont pas significatifs (p > 0.18), ce qui soutient l’hypothèse de tendances parallèles. Sans `same_switchers`, les résultats sont moins stables et certains placebos dérivent (ex. +288 avec large IC).