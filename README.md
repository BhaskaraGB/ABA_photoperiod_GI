This script performs an analysis of leaf temperature data collected from different genotypes under various photoperiods and treatments. It includes steps to clean the data, check statistical assumptions, perform repeated measures ANOVA, and visualize the results. The analysis follows these main steps:

Data Preparation: The script reads the data from a CSV file and selects relevant columns. It filters out the 'gi-100' genotype due to high variability in leaf temperature values.

Assumption Checks:

Outlier Identification: The script identifies and removes outliers.
Normality: The Shapiro-Wilk test is used to check the normality of the data.
Homogeneity of Variance: Levene's test checks the equality of variances.
Sphericity: Mauchly's test for sphericity is performed internally during the ANOVA test.
Statistical Analysis:

ANOVA: A repeated measures ANOVA is conducted to assess the effects of genotype, treatment, and photoperiod on leaf temperature.
Post-hoc Tests: Interaction effects and simple main effects are further analyzed using post-hoc tests.
Data Visualization:

Box Plots: Visualize the distribution of leaf temperatures across genotypes, treatments, and photoperiods.
Line Plots: Show the mean leaf temperatures with standard errors across different conditions.
Results: The analysis reveals significant interactions between genotype and photoperiod, and between treatment and photoperiod, with specific focus on the 'gi-2' mutant.

This script leverages R libraries such as tidyverse, ggpubr, and rstatix for data manipulation, statistical analysis, and visualization. The final visualizations are saved in both TIFF and SVG formats.






