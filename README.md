# Overview
This script performs a three-way mixed ANOVA and data visualization on leaf temperature (LT) data for different genotypes under varying photoperiods and treatments. It includes steps for identifying outliers, testing statistical assumptions, performing ANOVA, and creating visualizations. Find the published results of this analysis in this paper "GIGANTEA Is a Negative Regulator of Abscisic Acid Transcriptional Responses and Sensitivity in Arabidopsis"
https://academic.oup.com/pcp/article/63/9/1285/6647599

## Prerequisites
Ensure the following R packages are installed:

**tidyverse*
**ggpubr*
**rstatix*
**patchwork*

## Data Preparation: 
The script reads the data from a CSV file and selects relevant columns. It filters out the 'gi-100' genotype due to high variability in leaf temperature values.

## Assumption Checks:
**Outlier Identification**: The script identifies and removes outliers.

**Normality**: The Shapiro-Wilk test is used to check the normality of the data.

**Homogeneity of Variance**: Levene's test checks the equality of variances.

**Sphericity**: Mauchly's test for sphericity is performed internally during the ANOVA test.

## Statistical Analysis:
ANOVA: A repeated measures ANOVA is conducted to assess the effects of genotype, treatment, and photoperiod on leaf temperature.
Post-hoc Tests: Interaction effects and simple main effects are further analyzed using post-hoc tests.

## Data Visualization:
Box Plots: Visualize the distribution of leaf temperatures across genotypes, treatments, and photoperiods.

Line Plots: Show the mean leaf temperatures with standard errors across different conditions.

Results: The analysis reveals significant interactions between genotype and photoperiod, and between treatment and photoperiod, with specific focus on the 'gi-2' mutant.





