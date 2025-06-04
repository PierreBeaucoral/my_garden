---
{"dg-publish":true,"permalink":"/ph-d-thesis/chap-2/under-the-green-canopy-advancing-climate-finance-analysis-with-ai/"}
---



**Pierre Beaucoral**  
UCA CNRS IRD CERDI  
[pierre.beaucoral@uca.fr](mailto:pierre.beaucoral@uca.fr)

**Links:**  
- [Paper (PDF)](https://arxiv.org/pdf/<ARXIV_PAPER_ID>.pdf)  
- [Code (GitHub)](https://github.com/PierreBeaucoral/UNDERCANOPY)

---

## Abstract

Climate finance is critical for addressing the multifaceted challenges of climate change. This study employs **ClimateFinanceBERT**, a machine learning framework built on advanced NLP techniques, to re‐examine bilateral public climate finance flows. By classifying project descriptions from the OECD CRS dataset, our analysis refines estimates of both mitigation and adaptation finance, revealing that traditional methods may overestimate flows. The resulting insights offer an improved analytical framework for policymakers, emphasizing transparency and impact in climate finance allocation.

---

## Introduction

The escalating threat of climate change demands robust financial strategies. Traditional classification methods, such as the OECD’s Rio markers, have limitations that obscure the nuanced allocation of climate finance. This work introduces an AI-driven approach that leverages ClimateFinanceBERT to provide a more detailed and accurate estimation of bilateral public climate finance. By revisiting the determinants of climate finance allocation, we challenge longstanding assumptions and propose a framework that better aligns with contemporary climate challenges.

---

## Methods

### Data and Classification

Utilizing the OECD CRS dataset (1973–2022), the study examines over 5 million project descriptions. A two-stage classification using ClimateFinanceBERT first filters climate-relevant projects and then categorizes them into:
- **Mitigation**  
- **Adaptation**  
- **Environmental finance**

This approach incorporates modern NLP techniques and cluster analysis to overcome the biases inherent in self-reported data.

### Econometric Framework

A **double hurdle model** is employed to separately analyze:
1. **Selection stage**: the decision to allocate aid  
2. **Allocation stage**: the amount disbursed  

The model incorporates geopolitical, institutional, and vulnerability indicators, allowing for a nuanced understanding of both adaptation and mitigation finance determinants.

#### Full-Screen Flowchart

![Figure_1.png](/img/user/PhD%20Thesis/Chap%202/Figure_1.png)

---

## Results

The refined classification uncovers significant discrepancies between traditional CRS estimates and those produced by ClimateFinanceBERT. Key findings include lower estimates of mitigation and adaptation flows, suggesting that traditional methods may suffer from overreporting biases. The interactive visualizations below illustrate these differences, highlighting country vulnerabilities and the reclassified disbursement patterns.

---

### Graphical Carousel: First Set of Graphs

![Figure_A1.png](/img/user/PhD%20Thesis/Chap%202/Figure_A1.png)
*Map highlighting country vulnerability to climate risks*

![Figure_2.png](/img/user/PhD%20Thesis/Chap%202/Figure_2.png)
*Stackplot showing disbursement reclassified by ClimateFinanceBERT*

![Figure_3.png](/img/user/PhD%20Thesis/Chap%202/Figure_3.png)
*Stacked area chart comparing declaration of flows*

![Figure_4 1.png](/img/user/PhD%20Thesis/Chap%202/Figure_4%201.png)
*Projections*

---

## Econometric Analysis & Discussion

Using a double hurdle model, our analysis distinguishes between the selection and allocation stages of climate finance. For mitigation finance, a strong positive correlation suggests standardized decision-making, whereas adaptation finance displays a more complex, need-driven pattern. Tables and figures (not fully displayed here) quantify these effects, challenging traditional views on the role of historical ties and governance in climate aid distribution.

Below you can see:
- A **comparison by donor** of AI-based estimates versus traditional self-reported flows.  
- The **over-declaration ratio** for each donor country, illustrating how much traditional methods overstate climate finance.

---

### Graphical Carousel: Second Set of Graphs


![Figure_A3.png](/img/user/PhD%20Thesis/Chap%202/Figure_A3.png)  
*Comparison of study’s estimation vs. traditional methods by donor*

![Figure_A4.png](/img/user/PhD%20Thesis/Chap%202/Figure_A4.png)  
*Over-declaration ratio by donor countries*

---

## Policy Implications

The findings of this study have profound implications for international climate finance. With evidence of overreporting in traditional estimates, a shift toward transparency and impact-driven allocation is needed. Adaptation finance should be more focused on recipient vulnerability and institutional capacity, while mitigation finance remains partly influenced by historical ties. Tailored policy frameworks must recognize these differences to optimize financial flows and enhance the effectiveness of climate aid.

---

## BibTeX

```bibtex
@unpublished{beaucoral2025,
  title={Under the Green Canopy: Bringing Up to Date Public Climate Finance Determinants Analysis with AI},
  author={Beaucoral, Pierre},
  year={2025},
  note={Preliminary version. Supported by the Agence Nationale de la Recherche.},
  url={https://arxiv.org/abs/<ARXIV_PAPER_ID>}
}
