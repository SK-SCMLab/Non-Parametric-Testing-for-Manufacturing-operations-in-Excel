# 🪁 Non-Parametric-Testing-for-Manufacturing-operations-in-Excel
This repository contains case studies from real-world manufacturing environments, demonstrating how non-parametric tests can be carried out in manufacturing operations using Microsoft Excel including:

1. Mann-Whitney U test
2. Kruskal Wallis Test
3. Mood's Median test
4. Freidman Test
5. 1-Sample sign test
6. 1-Sample Wilcoxon test


            Note: - Non-parametric tests cannot be executed in Excel through straightforward functions. Hence, they require manual calculations within the Excel document
                  - For Mann-Whitney U test, users are supposed to refer to U-distribution table to determine the critical value 
   
---

## ⚽️ Non-parametric tests
Non-parametric tests do not make any assumptions about a distribution model where the data could fit. They compare groups of medians using the relative ranks of data within the groups. These graphs may skew right or skew left. Non-parametric tests are used when:

- Data **does not follow a normal distribution**
- Sample sizes are **small or uneven**
- Data is **ordinal** or has **outliers**
- We want to **compare medians or ranks** instead of means

These tests are powerful tools for robust, distribution-free inference, in real-world manufacturing scenarios where data violates parametric assumptions

---

## 🏀 Mann-Whitney U Test
Mann Whitney test is a non-parametric test used to compare the center between two unpaired groups. The obtained U has to be equal to or less than the critical value. 

---

## 🏈 Kruskal-Wallis Test 
The Kruskal-Wallis test is used for testing the source of origin of the samples. It is the only way to analyze the variance by ranks. The medians of two or more samples are compared to fixed the source of origin. It does not assume the normal distribution of the residuals

---

## ⚾️ Mood's Median test
The Mood's Median test is a non-parametric test that is used to test the equality of medians from two or more different population. The test works if:

      - The output (Y) variable is continuous, discrete-ordinal or discrete-count
      - The input (X) variable is discrete with two or more attributes

---

## 🎾 Freidman Test
The Freidman test is a form of non-parametric test that does not make any assumptions on the origin of the sample 

---

## 🏉 1-Sample Sign Test
1-Sample sign test is the simplest of all the non-parametric test that can be used instead of 1-sample test:

- Count the no of +ve values
- Count the no. of -ve values
- Test the values

---

## 🥏 1-Sample Wilcoxon test
1-Sample Wilcoxon test is a non-parametric test which is equivalent to 1-sample T.Test and is more powerful than 1-Sample Sign test. It is used to estimate the population median and compare it to target or reference value. It assumes the existing sample is randomly taken from a population

---

## 🏓 Case study: Non-parametric testing of Grinding machine in a steel manufacturing plant

### 🏏 Objectives

- Test whether two independent samples come from the same distribution (typically when normality can't be assumed) using Mann Whitney U test
- Test to compare three or more independent groups to assess whether their medians differ significantly using Kruskal-Wallis test (alternative to one-way ANOVA)
-  


---

### 🏸 Interpretation

1. *Situation: The factory operates two machines to carry out Grinding operation. They want to compare the output Width by each machine to determine if the output is uniform to one another*

   **Inference**: *Mann Whitney U Test* || From the excel analysis, U = 3 < 10 (U_Critical), we can reject H₀. It means that the data is not normally distributed. It can be used instead of 2-sample T.Test if normality/variance assumptions are violated

   **Conclusion**: There is statistically significant evidence that Machine A and Machine B of Grinding operation have different median output widths. Since A has lower output width comparatively in all ranks, it's likely more efficient


