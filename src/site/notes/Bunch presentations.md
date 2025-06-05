---
{"dg-publish":true,"permalink":"/bunch-presentations/"}
---


## UCA SEJPG JED (Journée Scientifique de l’École Doctorale SEJPG) 2024

The Journée Scientifique de l’École Doctorale SEJPG (JED SEJPG) is an annual gathering of doctoral students affiliated with the École Doctorale des Sciences Économiques, Juridiques, Politiques et de Gestion (SEJPG) at Université Clermont Auvergne (UCA). In 2024, the event took place on **13 June 2024**, in the lecture halls of the IADT building. It offers a platform for PhD candidates to present their research projects—either orally or as posters—and to exchange ideas in a collegial and interdisciplinary environment 

The primary goal of JED SEJPG is not only to showcase ongoing doctoral research but also to foster constructive dialogue; students are encouraged to “challenge” one another’s work in a spirit of mutual support rather than technical scrutiny. A jury composed of senior researchers from Clermont’s major laboratories evaluates the best oral presentations and posters, awarding prizes in different disciplines (Economics, Law & Political Science, Management). This year’s attendees included members of CERDI, CLErMa, CMH, LEO-UCA, and UMR Territoires, among others.

---

### My Poster Presentation: _“Cracking the Code: Enhancing Development Project Classification with NLP on OECD CRS Data”_

At JED SEJPG 2024, I presented my poster titled:

> **Cracking the Code: Enhancing Development Project Classification with NLP on OECD CRS Data**  
> Pierre Beaucoral (CERDI, UCA CNRS IRD)
> more about this in [[Projects\|Projects]]

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
