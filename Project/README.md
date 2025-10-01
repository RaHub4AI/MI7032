# Take-Home Exam Guidelines (2.5 credits)
  
**Exam period:** 27–31 October 2025  
- **Mid-exam presentations:** Wednesday, 29 October (09:00–17:00, Ahlmannsalen).  
- **Final submission deadline:** Friday, 31 October, 17:00 in **Athena**.  
- **Format:** Individual project submitted as a **Jupyter Notebook** (`.ipynb`) that combines text, code, figures, and outputs into a coherent and well-structured report.  

---

## Intended Learning Outcomes
After completing the course, students are expected to be able to:
1. **Select appropriate statistical methods** for descriptive statistics, hypothesis testing (parametric & non-parametric), correlation, and regression analysis of environmental data.  
2. **Apply statistical methods in R or Python** to real datasets.  
3. **Solve narrative data analysis problems** inspired by contemporary environmental research.  
4. **Present statistical results clearly, transparently, and formally correctly** in a reproducible research notebook.  

---

## Dataset Requirements
- You **must select your own dataset** (not personal/own-generated data).  
- The dataset must be **environmental** in nature (e.g., climate, air quality, water quality, biodiversity, land use, pollution, energy, etc.).  
- **Minimum size:** 200 observations and at least 4–5 relevant variables.  

### Possible Data Sources
- [Kaggle Datasets](https://www.kaggle.com/datasets)  
- [Hugging Face Datasets](https://huggingface.co/datasets)  
- [Bolin Centre Database (Sweden)](https://bolin.su.se/data)  
- [SMHI Climate Data](https://www.smhi.se/data)  
- [Eurostat Environment Data](https://ec.europa.eu/eurostat/data/database)  
- [Our World in Data](https://ourworldindata.org/)  
- Peer-reviewed research papers (with citation)  

To receive **feedback on dataset suitability**, submit your dataset choice in the shared **Google Drive table** before starting the analysis.  

---

## Mid-Exam Presentation (29 Oct)
- **5 minutes presentation** (slides optional, but strongly recommended).  
- Content must include:  
  - Project idea  
  - Dataset description (source, size, type of data)  
  - Statistical methods used so far & methods planned  
  - Justification: Why these methods are appropriate for your dataset  
- Followed by **peer + instructor feedback**  

---

## Minimum Technical Requirements
To pass, the final notebook **must include at least**:

### 1. Exploratory Data Analysis (EDA)
- One **summary table** (mean, median, sd, etc.)  
- At least **three different visualizations** (e.g., histogram, boxplot, scatterplot)  

### 2. Descriptive Statistics
- At least **two measures of central tendency** (mean, median, mode if relevant)  
- At least **two measures of variability** (variance, sd, IQR, etc.)  

### 3. Hypothesis Testing
- At least **two hypothesis tests**:  
  - One **parametric test** (*t*-test, ANOVA, etc.)  
  - One **non-parametric test** (Wilcoxon, Mann–Whitney, etc.)  
- Each test must include:  
  - Stated hypothesis (H₀, H₁)  
  - Justification of test choice (assumptions)  
  - Clear interpretation of results  

### 4. Correlation / Covariance
- At least **one correlation analysis** (Pearson, Spearman, or Kendall)  
- Visualization (scatterplot + correlation coefficient)  

### 5. Regression Analysis
- At least **one regression model** (linear or logistic)  
- Model summary + residual diagnostics  
- Interpretation of coefficients in environmental context  

### 6. Interpretation & Discussion
- Clear explanation of results in **words** (not just *p*-values)  
- Link back to the environmental research question  

### 7. Formatting & Reproducibility
- Notebook runs **without errors** from start to finish  
- All figures have **titles, axis labels, units**  
- Dataset and packages are cited  

---

## Jupyter Notebook Structure

Your `.ipynb` must follow this structure:

1. **Title Page**   
   - Project title, student name, course code, date  

2. **Introduction**  
   - Research problem/question  
   - Motivation & hypotheses  

3. **Dataset Description**  
   - Source + citation  
   - Description of variables  
   - Data cleaning steps  

4. **Exploratory Data Analysis (EDA)** 
   - Summary statistics table  
   - ≥3 plots  

5. **Statistical Analysis**  
   - ≥2 hypothesis tests (1 parametric, 1 non-parametric)  
   - ≥1 correlation analysis  
   - ≥1 regression analysis  

6. **Results & Interpretation** 
   - Clear written explanation of results with environmental relevance  

7. **Discussion**  
   - Limitations, reflections, environmental link  

8. **Conclusion**  

9. **References** 
   - Dataset(s), software packages, literature  

10. **Appendix (optional)**  
   - Additional code, diagnostics, or plots  

---

## Grading Criteria

| Category | Description | Weight | Minimum Requirement |
|----------|-------------|--------|---------------------|
| **Dataset & Relevance** | Environmental, appropriate size, well-documented | 10% | External dataset, ≥200 rows, ≥4–5 variables |
| **Research Question** | Clear, relevant, linked to environment | 10% | ≥1 research question + ≥1 hypothesis |
| **EDA & Descriptive Stats** | Summary + visualizations | 15% | ≥1 summary table, ≥3 plots, ≥4 descriptive measures |
| **Hypothesis Testing** | Correct selection + interpretation | 20% | ≥2 tests (1 parametric, 1 non-parametric) |
| **Correlation** | Application + interpretation | 10% | ≥1 correlation analysis with visualization |
| **Regression** | Application + interpretation | 15% | ≥1 regression model with coefficient interpretation |
| **Interpretation & Discussion** | Answers research questions, critical reflection | 10% | Results written in narrative, linked to context |
| **Presentation & Reproducibility** | Notebook clarity, formatting, references | 10% | Runs error-free, figures labeled, references present |

---

## Grading Scale
- **A (excellent):** Outstanding dataset choice, highly relevant research question, excellent application of methods, insightful interpretation, flawless reproducibility.  
- **B:** Very good analysis with minor shortcomings in clarity, interpretation, or formatting.  
- **C:** Good analysis with some gaps in methods or discussion.  
- **D:** Satisfactory; minimum criteria met but lacks depth.  
- **E:** Sufficient but superficial; errors in methodology or unclear results.  
- **Fx:** Major issues; can be improved with revisions.  
- **F:** Not acceptable; incomplete or off-topic.  

---

