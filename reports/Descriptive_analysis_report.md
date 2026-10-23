# Descriptive Analysis of Age and Sex Distribution in the UCI Heart Disease Dataset

**Analysis type:** Exploratory and descriptive data analysis  
**Dataset:** UCI Heart Disease Dataset  
**Sample size:** 303 participants  
**Tools:** Python, pandas, Matplotlib and Jupyter Notebook

---

## 1. Introduction

Exploratory data analysis (EDA) is an essential component of the data analytics workflow. It helps researchers understand the structure, distribution and characteristics of a dataset before undertaking more advanced statistical analyses or predictive modelling.

This report presents a descriptive analysis of age and sex among participants in the UCI Heart Disease dataset. The analysis uses summary statistics and graphical visualisations to describe the demographic composition of the dataset.

The work forms part of a practical Python data analytics project focused on data acquisition, descriptive statistics, visualisation and reproducible reporting.

## 2. Aim and Objectives

### 2.1 Aim

To describe the age and sex distribution of participants in the UCI Heart Disease dataset using descriptive statistics and data visualisation.

### 2.2 Specific objectives

1. To summarise the age distribution using measures of central tendency, variability and range.
2. To determine the frequency and percentage distribution of participants by sex.
3. To visualise age and sex distributions using appropriate graphical methods.
4. To interpret the findings and identify considerations for subsequent analyses.

## 3. Dataset and Analytical Methods

### 3.1 Dataset description

The analysis used the UCI Heart Disease dataset accessed through the `ucimlrepo` Python package. The version analysed contained 303 observations.

The analysis focused on two variables:

- **Age:** A numerical variable representing participant age in years.
- **Sex:** A categorical variable represented numerically in the source data and displayed using the corresponding category labels.

### 3.2 Software and libraries

The analysis was conducted in Python using Jupyter Notebook within Visual Studio Code. The following libraries supported the workflow:

- `ucimlrepo` — retrieval of the dataset from the UCI repository.
- `pandas` — data manipulation, frequency calculations and descriptive statistics.
- `Matplotlib` — generation and saving of graphical visualisations.
- `pathlib` — management of project directories and output file paths.

### 3.3 Statistical methods

Age was summarised using the number of observations, mean, standard deviation, minimum, maximum, median and interquartile range.

Sex distribution was described using frequency counts and percentages.

A histogram was used to visualise the distribution of age, while a bar chart was used to compare the number of participants in each sex category.

The figures were saved as PNG files in the project's `figures` directory. Summary tables were saved in the `reports` directory.

## 4. Results

### 4.1 Age distribution

The dataset contained 303 participants. Their mean age was 54.44 years, with a standard deviation of 9.04 years. The median age was 56 years, while the observed ages ranged from 29 to 77 years.

The first quartile was 48 years and the third quartile was 61 years. Consequently, the interquartile range was 13 years, indicating that the middle 50% of observed ages fell between 48 and 61 years.

**Table 1. Descriptive statistics for participant age**

| Statistic | Value |
|:---|---:|
| Number of participants | 303 |
| Mean age (years) | 54.44 |
| Standard deviation (years) | 9.04 |
| Minimum age (years) | 29 |
| 25th percentile (years) | 48 |
| Median age (years) | 56 |
| 75th percentile (years) | 61 |
| Maximum age (years) | 77 |
| Interquartile range (years) | 13 |

**Figure 1. Age distribution of participants in the UCI Heart Disease dataset.**

![Histogram showing the age distribution of participants](../figures/age_distribution.png)

The histogram shows that the observations are concentrated predominantly in middle and older adulthood. The tallest displayed histogram bin occurs around the late 50s to early 60s, suggesting that this interval contains the greatest number of observations among the displayed age bins.

The mean age of 54.44 years is slightly lower than the median age of 56 years. This difference may be consistent with some influence from lower-age observations, although the precise distributional shape should be assessed from the histogram and additional diagnostics rather than inferred from the mean and median alone.

Overall, the age statistics indicate that the dataset primarily represents adults in middle and older adulthood. This demographic composition is important when interpreting subsequent analyses of heart disease outcomes.

### 4.2 Sex distribution

The sex distribution showed that 206 participants were recorded as male, representing 67.99% of the dataset. The remaining 97 participants were recorded as female, representing 32.01%.

No observations were classified as unknown in the generated summary.

**Table 2. Distribution of participants by sex**

| Sex | Frequency | Percentage (%) |
|:---|---:|---:|
| Female | 97 | 32.01 |
| Male | 206 | 67.99 |
| Unknown | 0 | 0.00 |
| **Total** | **303** | **100.00** |

**Figure 2. Sex distribution of participants in the UCI Heart Disease dataset.**

![Bar chart showing the sex distribution of participants](../figures/sex_distribution.png)

The bar chart illustrates the unequal representation of the two recorded sex categories. Male participants constituted approximately two-thirds of the observations, whereas female participants accounted for approximately one-third.

This imbalance is an important characteristic of the dataset. In subsequent analyses comparing outcomes across sex categories, the different group sizes should be considered when interpreting estimates and uncertainty.

The observed distribution describes the dataset analysed; it does not establish that males have a higher prevalence or risk of heart disease than females. Such a conclusion would require a direct comparison of heart disease outcomes between the groups and careful consideration of the dataset's sampling and selection characteristics.

## 5. Discussion

This analysis provides an initial overview of the demographic composition of the UCI Heart Disease dataset.

The age analysis showed a mean age of 54.44 years and a median of 56 years, with an interquartile range of 13 years. The histogram further indicated that observations were concentrated in middle and older adulthood. These characteristics describe the age distribution of the available participants and provide context for examining clinical variables in later stages of the project.

The sex analysis identified a substantial imbalance between the recorded categories, with males accounting for 67.99% and females for 32.01% of the dataset. This imbalance may affect the precision of group-specific estimates in subsequent analyses, particularly if the outcome distribution differs between the categories.

Importantly, demographic distributions alone do not establish associations with heart disease. Although the dataset concerns heart disease, this stage of the project examined only age and sex as individual variables. No comparison of these variables against the heart disease outcome was performed.

The results therefore serve as a foundation for further exploratory analysis rather than as evidence of causal relationships or individual disease risk.

## 6. Limitations

Several limitations should be acknowledged when interpreting these findings.

1. **Representativeness:** The analysis describes the 303 observations in the version of the dataset used. The findings should not automatically be generalised to the wider population.

2. **Unequal sex distribution:** Male participants were more numerous than female participants. This imbalance should be considered when comparing clinical outcomes across sex categories.

3. **Limited variable scope:** Only age and sex were examined. Other clinical variables and the recorded heart disease outcome were not analysed in this report.

4. **Descriptive design:** The analysis summarises observed distributions and does not test statistical associations, establish causation or evaluate predictive performance.

5. **Variable coding:** The sex labels depend on the source variable's coding. The mapping should be verified against the metadata for the exact dataset version used.

6. **Visual interpretation:** The histogram provides a visual overview of age distribution, but the precise shape depends partly on the selected bin widths. Additional diagnostics may be needed to assess skewness, unusual observations or distributional assumptions.

## 7. Conclusion

The descriptive analysis characterised the age and sex distribution of 303 participants in the UCI Heart Disease dataset.

The mean age was 54.44 years, the median was 56 years, and ages ranged from 29 to 77 years. The middle 50% of participants were aged between 48 and 61 years. Males represented 67.99% of the dataset, compared with 32.01% females.

The summary statistics and visualisations provide a clear initial understanding of the dataset's demographic composition. These findings establish a foundation for further exploratory work, particularly analysis of the recorded heart disease outcome across age groups and sex categories.

The results should be interpreted as descriptions of the analysed dataset, not as estimates of population-level demographics or evidence of differences in heart disease risk.

## 8. Reproducibility and Project Outputs

The analysis was performed in a Jupyter Notebook using Python. The following project outputs document the work:

| File | Description |
|:---|:---|
| `figures/age_distribution.png` | Histogram of participant age |
| `figures/sex_distribution.png` | Bar chart of participant sex |
| `reports/age_summary_statistics.csv` | Summary statistics for age |
| `reports/sex_distribution_summary.csv` | Sex frequencies and percentages |
| `reports/descriptive_analysis_report.md` | Written descriptive analysis report |

The figures are referenced using relative paths so they can be displayed directly in the Markdown preview and on GitHub when the project directory structure is preserved.

The notebook and supporting outputs should be maintained together in the project repository to support transparency, reproducibility and future extension of the analysis.

## 9. Next Steps

The next stage of the project should focus on:

1. Inspecting the recorded heart disease outcome and its coding.
2. Examining the frequency distribution of outcome categories.
3. Comparing age distributions between outcome groups.
4. Comparing outcome frequencies across sex categories.
5. Developing additional visualisations based on the findings and documenting the results.

These analyses would extend the current demographic description while preserving a clear distinction between descriptive patterns and statistical evidence of associations.
