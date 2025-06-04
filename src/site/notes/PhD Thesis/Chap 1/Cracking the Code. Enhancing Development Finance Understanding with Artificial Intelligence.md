---
{"dg-publish":true,"permalink":"/ph-d-thesis/chap-1/cracking-the-code-enhancing-development-finance-understanding-with-artificial-intelligence/"}
---




**Pierre Beaucoral**<sup>*</sup>  
UCA CNRS IRD CERDI  
[pierre.beaucoral@uca.fr](mailto:pierre.beaucoral@uca.fr)

<sup>*</sup>Indicates Equal Contribution

**Links:**  
- [Paper (PDF)](https://arxiv.org/pdf/2502.09495.pdf)  
- [Code (GitHub)](https://github.com/PierreBeaucoral/ML-clustering-of-development-activities)  
- [arXiv](https://arxiv.org/abs/2502.09495)

---

## Abstract

This study leverages advanced AI techniques to analyze almost 5 million project narratives from the OECD CRS dataset. By combining BERT-based text embedding, HDBSCAN clustering, and automated labeling with Class-based TF-IDF and LLM fine-tuning, I uncover 406 hidden thematic clusters in development finance. Our results reveal discrepancies in traditional classifications and offer a refined lens on donor priorities and aid effectiveness.

---

## Introduction

In an era of data-driven decision-making, understanding the intricacies of development finance is critical. This research addresses key questions such as: *How can machine learning improve the classification of development projects?* and *What hidden themes exist beyond traditional OECD classifications?* The objective of this research is to propose an AI-driven framework that enhances the transparency and precision of public and private aid analysis.

---

## Related Work

Previous studies have predominantly relied on self-declared project classifications and predefined sectors, which can obscure nuanced thematic distinctions. Recent advances in Natural Language Processing and Machine Learning now allow for a more granular examination. Our approach builds upon these developments, bridging existing gaps in the literature regarding aid effectiveness and donor-recipient dynamics. This research is based on the seminal paper by Toetzke et al. (2022).

---

## Methodology

### Data Collection & Preprocessing

- Over 5 million project descriptions were extracted from the OECD CRS dataset.  
- Rigorous cleaning and quality control procedures were implemented to ensure reliable inputs for analysis.

### Text Embedding & Clustering

- We utilized a BERT-based transformer model to convert narrative descriptions into dense vector representations.  
- The HDBSCAN clustering algorithm then grouped these vectors into 406 distinct thematic clusters, providing a more detailed classification than traditional methods.

### Automated Labeling

- Clusters were automatically labeled using a combination of Class-based TF-IDF and fine-tuning with large language models.  
- We used the LLM **Zephyr-7Bβ** (a fine-tuned version of Mistral-7B-v0.1) to generate descriptive and interpretable thematic tags.

### Interactive Visualization

Interactive outputs visualize clustering results and thematic distributions. These visualizations enable exploration of trends over time, donor-recipient relationships, and thematic overlaps across projects.

---

## Interactive Outputs

- **Topic frequency through years**: [View visualization](topics_over_time_visualization.html)  
- **Topic frequency per donor**: [View visualization](topics_per_donor_visualization.html)  
- **Commitments for topics through years**: [View visualization](commitmentyear_plot.html)  

---

## Results

- **Uncovering Hidden Themes:** The identification of 406 distinct clusters reveals subtle thematic nuances that traditional classifications miss.  
- **Enhanced Transparency:** Interactive visualizations provide a dynamic view of donor priorities and aid flows, supporting data-driven insights.  
- **Comparative Analysis:** Our method highlights discrepancies between AI-based classifications and conventional OECD categorizations, offering a more nuanced analysis of project objectives.

Below are some visual results:

![Great Apes Conservation Projects](/img/user/Figure_6.png)  
*Great Apes Conservation Projects*


![Syrian Conflict Projects](/img/user/Figure_7.png)  
*Syrian Conflict Projects*

![Aid Trends Analysis](/img/user/Figure_8.png)  
*Aid Trends Analysis*

---

## Discussion & Conclusion

Our findings underscore the limitations of traditional classification methods in capturing the complexity of development finance. The AI-driven approach not only refines thematic categorization but also provides actionable insights for policymakers. While our results are promising, further work is needed to integrate additional data sources and validate the findings across varied contexts.

Future research directions include the incorporation of real-time data and expanding the analysis to encompass more dynamic elements of global aid distribution.

---

## BibTeX

```bibtex
@misc{beaucoral2025crackingcodeenhancingdevelopment,
  title={Cracking the Code: Enhancing Development Finance Understanding with Artificial Intelligence}, 
  author={Pierre Beaucoral},
  year={2025},
  eprint={2502.09495},
  archivePrefix={arXiv},
  primaryClass={econ.GN},
  url={https://arxiv.org/abs/2502.09495},
}
