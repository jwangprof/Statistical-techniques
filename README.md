# Statistical-techniques
Statistical techniques are methods used to analyze, interpret, and draw conclusions from data. These techniques are vital in both descriptive and inferential statistics, helping us understand patterns, relationships, and trends in datasets. Here are some of the most commonly used statistical techniques across different domains:
### Summary of Common Statistical Techniques

| **Technique**               | **Purpose**                                                   |
|-----------------------------|---------------------------------------------------------------|
| **Descriptive Statistics**   | Summarize the main characteristics of the dataset             |
| **Hypothesis Testing**       | Test assumptions or differences between groups                |
| **Regression Analysis**      | Model relationships between dependent and independent variables|
| **Correlation Analysis**     | Measure the strength of relationships between variables       |
| **Non-Parametric Tests**     | Perform tests without assuming normality                      |
| **Time Series Analysis**     | Analyze data points collected over time                       |
| **Dimensionality Reduction** | Reduce the number of variables                                |
| **Clustering**               | Group data into similar clusters                              |
| **Bayesian Inference**       | Update probabilities based on prior knowledge                 |
| **Bootstrapping**            | Resample data to estimate statistical measures                |

### **1. Descriptive Statistics**
Descriptive statistics summarize and describe the features of a dataset, providing a snapshot of the data.

- **Measures of Central Tendency**:
  - **Mean**: The average of the dataset.
  - **Median**: The middle value when data is ordered.
  - **Mode**: The most frequent value in the dataset.

- **Measures of Variability**:
  - **Variance**: The average squared difference between each data point and the mean.
  - **Standard Deviation**: The square root of variance, it indicates how spread out the data is.
  - **Interquartile Range (IQR)**: The range between the 25th percentile (Q1) and 75th percentile (Q3), used to measure the spread of the middle 50% of the data.

- **Distribution Shape**:
  - **Skewness**: Measures the asymmetry of the distribution.
  - **Kurtosis**: Measures the "tailedness" of the distribution, identifying whether it has heavy or light tails.

---

### **2. Inferential Statistics** - **Also used for feature selection**
Inferential statistics are used to make inferences or predictions about a population based on a sample.

- **Hypothesis Testing**:
  - **Null Hypothesis (H₀)**: Assumes no effect or no difference.
  - **Alternative Hypothesis (H₁)**: Assumes there is an effect or difference.
  - **p-value**: The probability of observing the data if the null hypothesis is true. If the p-value is less than a significance level (usually 0.05), the null hypothesis is rejected.


 **F-test, t-test, ANOVA, and Chi-square test can be used for feature selection in machine learning models, especially when you're evaluating the relationship between independent variables (features) and the dependent variable (target)**
- **T-tests**:
  - **One-sample t-test**: Tests if the mean of a single group is different from a known value.
  - **Independent t-test**: Compares the means of two independent groups.
  - **Paired t-test**: Compares the means of two related groups (e.g., before and after treatment).

- **ANOVA (Analysis of Variance)**:**Tests for significant differences in means across multiple groups**.
  - **One-way ANOVA**: Tests differences in means across one categorical variable.
  - **Two-way ANOVA**: Tests the effect of two factors on a continuous outcome.

- **Chi-Square Test**:
  - **Chi-Square Test of Independence**: Tests whether two categorical variables are independent.
  - **Chi-Square Goodness of Fit Test**: Tests how well observed data fits a particular distribution.

---
### 3. Non-Parametric Tests

- **Non-parametric tests** do not assume the data follows a specific distribution and are used when data violates assumptions of parametric tests (like normality).

   1. **Mann-Whitney U Test**: A non-parametric alternative to the independent t-test.
   2. **Wilcoxon Signed-Rank Test**: A non-parametric test for paired data, used instead of the paired t-test.
   3. **Kruskal-Wallis Test**: A non-parametric version of ANOVA, used to compare more than two groups.
   4. **Friedman Test**: A non-parametric alternative to repeated-measures ANOVA.









