---
{"dg-publish":true,"permalink":"/academic-life/bunch-presentations/"}
---

## UCA SEJPG JED (Journée Scientifique de l’École Doctorale SEJPG) 2024

The Journée Scientifique de l’École Doctorale SEJPG (JED SEJPG) is an annual gathering of doctoral students affiliated with the École Doctorale des Sciences Économiques, Juridiques, Politiques et de Gestion (SEJPG) at Université Clermont Auvergne (UCA). In 2024, the event took place on **13 June 2024**, in the lecture halls of the IADT building. It offers a platform for PhD candidates to present their research projects—either orally or as posters—and to exchange ideas in a collegial and interdisciplinary environment 

The primary goal of JED SEJPG is not only to showcase ongoing doctoral research but also to foster constructive dialogue; students are encouraged to “challenge” one another’s work in a spirit of mutual support rather than technical scrutiny. A jury composed of senior researchers from Clermont’s major laboratories evaluates the best oral presentations and posters, awarding prizes in different disciplines (Economics, Law & Political Science, Management). This year’s attendees included members of CERDI, CLErMa, CMH, LEO-UCA, and UMR Territoires, among others.

---

### My Poster Presentation: _“Cracking the Code: Enhancing Development Project Classification with NLP on OECD CRS Data”_

At JED SEJPG 2024, I presented my poster titled:

> **Cracking the Code: Enhancing Development Project Classification with NLP on OECD CRS Data**  
> Pierre Beaucoral (CERDI, UCA CNRS IRD)
> more about this in [[Academic life/Projects\|Projects]]

This research addresses a critical challenge in development economics: accurately categorizing projects in the OECD Creditor Reporting System (CRS) dataset. While CRS provides a comprehensive repository of over five million development project descriptions, its sectoral and thematic coding relies on donor‐declared objectives, which can be inconsistent or incomplete. My poster outlines a novel, unsupervised Natural Language Processing (NLP) workflow using BERTopic to cluster projects based on their narrative descriptions, thereby revealing more fine‐grained thematic groupings than standard CRS codes allow.

### Reflections from JED SEJPG 2024
Presenting at JED SEJPG was an invaluable opportunity to receive feedback from experts in development economics and AI. During the poster session, I discussed:
- **LLM‐Based Labeling:**  
  While Zephyr‐7B-β generated coherent topic names in French, I was encouraged to trial alternative prompts to ensure consistency across languages.

- **Future Directions:**  
  - Linking clusters to financial flows over time to track the evolution of donors’ climate finance priorities.  

Overall, the event’s constructive atmosphere and interdisciplinary jury helped refine my methodology and inspired collaborative next steps.

---

![Capture d’écran 2025-06-05 à 11.01.27.png](/img/user/Capture%20d%E2%80%99%C3%A9cran%202025-06-05%20%C3%A0%2011.01.27.png)

--- 
## R Programming for Beginners (Sep 10, 2024)
On September 10, 2024, I delivered an **18-hour introductory course on R** designed for participants with no prior experience in data analysis. The course was structured into **six 3-hour sessions**, each focusing on core skills needed to load, manipulate, and visualize data using R. 

---
### Course Objectives

1. **Familiarize students with the R environment**: 
   - Installing R and RStudio  
   - Understanding the R console, script editor, and workspace

2. **Load and inspect datasets**:  
   - Reading CSV, Excel, and text files  
   - Exploring data frames, checking data structure, and handling missing values

3. **Perform basic statistical analyses**:  
   - Descriptive statistics (mean, median, standard deviation, quantiles)  
   - Simple hypothesis tests (t-tests, chi-square tests)  
   - Basic linear regression

4. **Create data visualizations**:  
   - Generating plots with base R (histograms, scatterplots, boxplots)  
   - Introduction to the **ggplot2** grammar of graphics (bar charts, line graphs, customized themes)

5. **Write reproducible code**:  
   - Organizing scripts into modular sections  
   - Using comments and naming conventions for clarity  
   - Saving and exporting results (tables, figures)

6. **Build a foundation for further study**:  
   - Providing guidance on advanced topics (data wrangling with `dplyr`, interactive dashboards with `Shiny`, and statistical modeling with `caret`)  
   - Sharing resources and best practices for continued learning
---
### Session Breakdown
1. **Session 1: Introduction to R & RStudio**  
   - Installing R and RStudio  
   - Navigating the interface  
   - Using basic commands and help functions  
   - Loading datasets from CSV files

2. **Session 2: Data Exploration & Manipulation**  
   - Inspecting data frames (`str()`, `summary()`, `head()`)  
   - Subsetting rows and columns  
   - Handling missing values and data types  
   - Installing and loading additional packages

3. **Session 3: Descriptive Statistics & Basic Tests**  
   - Calculating means, medians, standard deviations, and quantiles  
   - Creating frequency tables and cross-tabulations  
   - Performing t-tests and chi-square tests  
   - Interpreting p-values and confidence intervals

4. **Session 4: Introduction to ggplot2**  
   - Grammar of graphics: `aes()`, `geom_*()` functions  
   - Building scatterplots, histograms, and boxplots  
   - Customizing axes, labels, and themes  
   - Saving plots to files

5. **Session 5: Basic Linear Regression**  
   - Fitting a linear model with `lm()`  
   - Interpreting coefficients, R-squared, and p-values  
   - Plotting regression lines and diagnostic plots  
   - Exporting regression summaries and plots

6. **Session 6: Putting It All Together**  
   - Working through a complete example analysis  
   - Combining data import, cleaning, analysis, and visualization  
   - Discussion of reproducible research best practices  
   - Q&A and next steps for advanced learning
---
### Required Materials
All participants were provided with the following files before the first session:
- **Sample datasets (Data.zip)**:  
  Download the CSV and Excel files used for hands-on exercises:  
  [Download Data](https://pierrebeaucoral.github.io/course/r-for-beginners/Data.zip) 
- **Course slides & code (R-for-Beginners.zip)**:  
  Contains annotated R scripts, presentation slides, and explanation notebooks:  
  [Download Course Code and Slides](https://pierrebeaucoral.github.io/course/r-for-beginners/R-for-Beginners.zip) 
---
### Reflections & Feedback
**Engagement:**  
- Attendees ranged from complete beginners (no programming experience) to those with minimal exposure to Excel macros. By structuring the sessions incrementally, everyone could follow along and build confidence.
**Highlights:**  
- **Interactive exercises**: Using real‐world datasets (e.g., economic indicators, survey data), participants practiced writing scripts to calculate summary statistics and plot trends.  
- **Live coding**: Demonstrating code changes in real time helped students see how errors manifest and how to debug.  
- **Peer learning**: Breakout discussions allowed participants to compare approaches, reinforcing the idea that there are often multiple ways to achieve the same result in R.
**Challenges:**  
- Some attendees struggled with R’s object‐oriented syntax initially, especially when transitioning from Excel. To address this, I provided an optional appendix covering R fundamentals after Session 2.  
- Time constraints meant that not everyone could complete every exercise in class. I assigned additional practice problems for self-study between sessions.
**Outcomes:**  
- By the end of the 18 hours, all participants were able to:  
  - Import their own datasets into R  
  - Compute and interpret basic statistics  
  - Produce publication-quality plots with ggplot2  
  - Fit and evaluate a simple linear regression model  
- Several students expressed interest in exploring data wrangling with `dplyr` and creating interactive Shiny apps, setting the stage for potential follow-up workshops.
---
### Resources & Next Steps
For those who wish to continue advancing their R skills, I recommend:
- **“R for Data Science” by Hadley Wickham & Garrett Grolemund**: A free online book covering data manipulation (`dplyr`), visualization (`ggplot2`), and more.  
- **CRAN Task Views**: Browse topic-specific packages (e.g., “Econometrics,” “Spatial Data Analysis”) to find tools suited to your research needs.  
- **Swirl**: An in‐console interactive tutorial (`install.packages("swirl")`) for practicing R fundamentals.  
- **RStudio Community Forums**: Post questions or browse solutions when you encounter difficulties.  
---
Some of their graphs are available [here](https://pierrebeaucoral.github.io/post/gpe/)

## Journée Audaces 

#french 

Aujourd'hui, j’ai eu le plaisir de participer à la 12ᵉ Journée AuDACES, qui s’est tenue à l’Amphi Recherche des Cézeaux sur le campus des Cézeaux à Clermont-Ferrand. Organisée chaque année par le réseau AuDACES (AUvergne Développement d’Applications et Calcul en Environnement Scientifique), cette rencontre a pour objectif de favoriser les échanges entre chercheurs, ingénieurs et étudiants autour des avancées en intelligence artificielle (IA). La journée a rassemblé  plusieurs interventions couvrant aussi bien l’application de l’IA en finance, en robotique agricole, que son usage dans les sciences humaines et sociales (SHS).
### **Ma participation : contexte et motivations**  
En tant que doctorant en économie du développement au CERDI (Centre d’Études et de Recherche sur le Développement International), j’ai proposé une présentation intitulée :

> _“Intelligence Artificielle dans la recherche en SHS : intérêt, perspectives et applications”_

Mon intervention s’inscrivait dans la session consacrée à l’IA appliquée à des domaines très variés. L’objectif principal était de montrer comment des techniques de traitement automatique du langage (NLP) et de machine learning peuvent enrichir les approches classiques en SHS, en illustrant par deux projets menés dans le cadre de ma thèse. Pour moi, cette journée était l’opportunité de présenter un panorama des potentialités de l’IA dans les disciplines qui étudient la réalité humaine (économie, sociologie, anthropologie, etc.) et d’échanger avec des chercheurs issus d’autres équipes clermontoises, notamment celles du LIMOS, du LaMP ou du Mésocentre.

### **Présentation de mon profil et de ma recherche**  
J’explique souvent que, malgré ma formation d’économiste, j’ai progressivement intégré des méthodes d’apprentissage automatique (ML) et de NLP pour analyser de très gros corpus textuels (projets d’aide, rapports officiels, etc.). L’enjeu est de déceler des schémas thématiques fins – souvent masqués par les classifications officielles (codes secteurs, marqueurs Rio) – et de mesurer avec plus de précision la part réellement dédiée au climat dans les financements internationaux.

Par cette présentation, je voulais montrer que, si l’IA est souvent associée aux sciences exactes ou à l’ingénierie, elle trouve aussi un intérêt croissant dans les SHS, où elle permet d’explorer des corpus de textes ou d’images à une échelle inédite.

### **Intérêts de l’IA en SHS : automatisation et nouveaux traitements de données**  
Pour structurer mon propos, j’ai distingué deux grands axes :

1. **Automatisation des tâches répétitives et volumineuses**
    - Analyse d’archives : on peut désormais traiter des corpus historiques ou administratifs énormes pour extraire des informations (dates, lieux, acteurs, catégories d’événements) sans y passer des mois en travail manuel.
    - Classification automatisée : les modèles non supervisés (clustering) ou supervisés (classifieurs) facilitent la catégorisation à grande échelle (par exemple, thématiser automatiquement des projets d’aide à travers le monde).
    - Revue de littérature et gestion bibliographique : des outils de NLP permettent d’identifier les articles académiques pertinents, d’extraire des résumés automatiques, voire de proposer une arborescence thématique pour guider la recherche documentaire.  
    
    Au final, l’IA se présente comme un assistant de recherche personnalisé, capable de soulager le chercheur SHS de tâches mécaniques et chronophages.
    
2. **Exploration de nouvelles formes de données**
    
    - **Analyse de textes et d’images** : jusqu’à récemment, un historien ou un anthropologue avait parfois du mal à traiter automatiquement des photographies, des cartes anciennes ou des fichiers audio pour en extraire des tendances statistiques ; aujourd’hui, des algorithmes de détection d’objets, de classification d’images ou de reconnaissance vocale ouvrent un champ de possibles considérable.
    - **Imputation de données manquantes** : beaucoup de données d’enquête en SHS souffrent d’incomplétudes (non-réponse, données égarées) ; des méthodes de ML (KNN, autoencodeurs, forêts aléatoires) permettent d’estimer les valeurs manquantes pour préserver la qualité des analyses quantitatives.
    - **Génération de contenu synthétique (“expected parrots”)** : les LLM peuvent simuler des réponses à des questionnaires selon le contexte sociologique, ce qui aide à tester des enquêtes ou à vérifier la cohérence interne des réponses (par exemple, détecter si une série de réponses libres est juste un copié-collé de formules trop génériques).
        

### **Application possible**

J'ai pu parlé de deux projets de recherche [[Academic life/PhD Thesis/Chap 1/Cracking the Code. Enhancing Development Finance Understanding with Artificial Intelligence\|Cracking the Code. Enhancing Development Finance Understanding with Artificial Intelligence]] et [[Academic life/PhD Thesis/Chap 2/Under the Green Canopy. Advancing Climate Finance Analysis with AI\|Under the Green Canopy. Advancing Climate Finance Analysis with AI]]. Ainsi que d'autres pistes. 

**Autres pistes et applications possibles**  
Pour conclure mon intervention, j’ai évoqué quelques autres perspectives d’application de l’IA en SHS :

- **Analyse d’images à visée géopolitique** : par exemple, détection d’infrastructures stratégiques (cuves de stockage, sites industriels) à partir d’imagerie satellite (réseaux CNN, YOLOX-TR).
- **Traitement de données d’enquêtes** : imputation automatique de valeurs manquantes (KNN, autoencodeurs) et usage de LLM pour enrichir des réponses libres (par exemple, compléter une instruction “Bac + 2” en précisant l’année ou la filière).
- **Analyse de sentiment** dans de larges corpus de réponses ouvertes (lexiques, SVM, BERT) pour mesurer l’attitude collective vis-à-vis de sujets variés (politiques publiques, produits culturels, etc.).

>J’ai insisté sur les **opportunités** (gain d’échelle, objectivité, granularité) mais aussi sur les **limites** : méfiance des chercheurs SHS préoccupés par une “boîte noire” incompréhensible, biais potentiels dans les LLM reproduisant stéréotypes culturels, ou phénomène d’“expected parrot” qui peut générer des réponses trop génériques sans valeur ajoutée.

**Temps d’échanges et retours**  
La session a duré environ 30 minutes. Parmi les discussions, certains collègues du LIMOS ou du LaMP se sont montrés particulièrement intéressés par l’aspect « intérêt de ces outils pour les SHS » : j’ai pu échanger avec eux sur les difficultés liées à la constitution d’un sous-corpus labellisé et sur la question du coût de calcul (accès aux GPU via le Mésocentre). 

**Conclusion et remerciements**  
Cette Journée AuDACES m’a permis de :
- Mettre en lumière le rôle croissant de l’IA dans les SHS,
- Partager des retours d’expérience concrets issus de ma thèse,
- Tisser des liens avec des équipes clermontoises spécialisées dans l’IA appliquée à d’autres domaines.

Je tiens à remercier chaleureusement le réseau AuDACES pour l’organisation, AMD pour le déjeuner, et le CERDI. Enfin, je remercie tous les participants pour leurs questions pertinentes et leurs suggestions d’amélioration. J’espère que ces échanges feront naître de nouvelles collaborations interdisciplinaires : l’IA en SHS est un terrain en pleine expansion, et la Journée Audaces était l’occasion idéale pour mesurer l’étendue des possibles et identifier des synergies entre acteurs locaux. Ma présentation:
[Intelligence Artificielle dans la recherche en SHS.pdf](https://drive.uca.fr/f/e6f50a953f524000b78c/)
