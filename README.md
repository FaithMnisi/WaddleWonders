# WaddleWonders 🐧

## Overview

This project performs an Exploratory Data Analysis (EDA) on a penguin dataset, exploring biometric measurements (culmen length, culmen depth, flipper length, body mass) and categorical variables like species, island, and sex. The goal is to uncover patterns, relationships, and trends in the dataset to gain insights into penguin morphology and ecology.

## Dataset

The dataset includes the following features:

- **species**: The species of penguin (Adelie, Chinstrap, Gentoo)
- **island**: The island where the penguins were observed (Torgersen, Biscoe, Dream)
- **culmen_length_mm**: Length of the upper bill (in mm)
- **culmen_depth_mm**: Depth of the upper bill (in mm)
- **flipper_length_mm**: Length of the flipper (in mm)
- **body_mass_g**: Weight of the penguin (in grams)
- **sex**: Gender of the penguin (Male, Female)

## Analysis Goals

- **Correlation Analysis**: Explore the relationships between biometric measurements (culmen length, culmen depth, flipper length, body mass) using a heatmap to identify potential patterns and associations.
  
- **Distribution Exploration**: Visualize the distribution of biometric measures across penguin species using box plots. This helps elucidate potential differences or similarities in species-specific traits, which may reflect adaptations to ecological conditions, foraging strategies, and evolutionary factors.

- **Sexual Dimorphism**: Investigate gender-based differences in biometric measurements using scatter glyphs to visualize size and morphology differences between male and female penguins. This analysis also includes validation with box plots and t-tests to quantify the significance of these observed differences.

- **Island-Specific Differences**: Use ANOVA analysis to assess whether biometric measurements differ significantly across the three islands (Torgersen, Biscoe, Dream), highlighting potential island-specific patterns influenced by environmental conditions.

## Techniques Employed

- **Data Cleaning**: 
  - Removed duplicate rows using the `drop_duplicates()` function in Pandas.
  - Identified and removed missing data, particularly in the 'sex' column.
  
- **Exploratory Data Analysis**:
  - **Correlation Analysis**: Explored relationships between biometric measurements using a heatmap.
  - **Distribution Exploration**: Visualized the distribution of biometric measurements across penguin species using boxplots.
  - **Sexual Dimorphism**: Investigated gender-based differences in biometric measurements using scatter glyphs, box plots, and t-tests.
  - **ANOVA Analysis**: Analyzed biometric measurements across different islands to identify island-specific variations.

## Methodology

- **Tools**: Python, Pandas, Numpy, Seaborn, Matplotlib
- **Key Visualizations**:
  - **Heatmap**: Used for correlation analysis to reveal relationships between biometric measurements.
  - **Boxplot**: Used to compare distributions of biometric measures across species, uncovering species-specific traits.
  - **Scatter Glyph**: Visualized the relationship between biometric measurements for males and females to explore sexual dimorphism.
  - **Boxplot and T-tests**: Validated findings from scatter glyphs by providing data distribution details and quantifying the significance of gender differences.
  - **ANOVA**: Applied to assess differences in biometric measurements across islands.

## Key Findings

- **Correlations**:
  - **Culmen length** and **culmen depth**: Weak negative correlation of -0.23.
  - **Culmen length** and **flipper length**: Strong positive correlation of 0.65.
  - **Culmen length** and **body mass**: Strong positive correlation of 0.59.
  - **Culmen depth** and **flipper length**: Strong negative correlation of -0.58.
  - **Culmen depth** and **body mass**: Moderate negative correlation of -0.47.
  - **Flipper length** and **body mass**: Very strong positive correlation of 0.89.
  
- **Species-Specific Insights**:
  - **Adelie** and **Chinstrap** penguins have similar median **culmen lengths** and **culmen depths**, with Adelie's distribution skewing lower.
  - **Gentoo** penguins have considerably larger **flipper lengths** compared to Adelie and Chinstrap, with a median of ~216 mm.
  - **Adelie** and **Chinstrap** penguins share a similar median body mass of ~3700-3950 g.
  
- **Sexual Dimorphism**: 
  - Males tend to have greater biometric measurements (larger size, longer bills, and flippers) compared to females.

- **Island-Specific Patterns**:
  - The **Torgersen** island penguins had slightly larger **body mass** on average compared to the other islands.

## Conclusion

This analysis provides a comprehensive overview of the relationships between key biometric features of penguins across species, gender, and island, highlighting significant trends and insights.
