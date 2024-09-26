# Statistical-techniques
Statistical techniques are methods used to analyze, interpret, and draw conclusions from data. These techniques are vital in both descriptive and inferential statistics, helping us understand patterns, relationships, and trends in datasets. Here are some of the most commonly used statistical techniques across different domains:

---
### Check Statistical Test Assumptions
1. Linearity: Residual vs. Fitted Plot: A visual diagnostic to check if the relationship between the independent and dependent variables is linear. If the residuals show no discernible pattern, the assumption of linearity holds.

2. Assumptions of Normality: Many statistical tests require the data to be normally distributed. Tools like Shapiro-Wilk’s W test and Kolmogorov-Smirnov test, along with skewness and kurtosis measures, are instrumental in assessing this assumption. Graphical methods, such as Q-Q plots, also provide visual confirmation of normality.

What Happens If the Residual Assumptions Are Violated?

- 1. Non-linearity: You might need to try a more flexible model (e.g., polynomial regression or splines) or transform the independent variables.

- 2. Heteroscedasticity: Apply a transformation to the dependent variable (e.g., log or square root) or use models that can handle non-constant variance, such as generalized least squares (GLS).

- 3. Non-Normal Residuals: A non-normal distribution may require transformation of the dependent variable or the use of a robust regression model.
Autocorrelation: You might need to consider time series models like ARIMA if residuals are correlated in a time-dependent manner.

3. Homogeneity of Variance: Levene’s test is commonly used to ensure that different groups have equal variances, a condition necessary for various analysis techniques.

3. Homogeneity of Variance-Covariance Matrices: Box’s M test evaluates if groups differ in their variance-covariance matrices, an essential assumption for multivariate analysis.

4. Randomness: The assumption that sample observations are random is fundamental, with the Run Test serving as a method to confirm this condition.

5. Multicollinearity: High correlation among independent variables can distort regression analysis. The Variance Inflation Factor (VIF) and Condition Indices are tools used to detect multicollinearity, with VIF values greater than 10 indicating a violation of this assumption.
---

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

---
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

### Summary of Common Data issues

| **Common Data Issue**       | **How to Handle**                                             |
|-----------------------------|---------------------------------------------------------------|
| **Missing Data**            | Imputation, removal, flagging                                 |
| **Duplicated Data**         | Remove duplicates                                             |
| **Outliers**                | Remove, Winsorize, or transform                               |
| **Inconsistent Data**       | Standardize categories, formats                               |
| **Skewness**                | Apply log, square root, or Box-Cox transformation             |
| **Multicollinearity**       | Remove variables, regularization, PCA, Lasso/Ridge                         |
| **Imbalanced Data**         | Resampling (SMOTE), use class weights                         |
| **Scaling Data**            | StandardScaler, MinMaxScaler                                  |
| **Categorical Data**        | One-hot encoding, label encoding                              |
| **Data Leakage**            | Careful data splitting, avoid future data leakage             |
| **Class Imbalance**         | Use oversampling/undersampling, class weights                 |
| **High Dimensionality**     | PCA, feature selection                                        |
| **Feature Engineering**     | Create new features, extract meaningful information           |
| **Irrelevant Features**     | Feature selection techniques                                  |
| **Temporal Data Issues**    | Maintain time order, use time-aware features                  |







