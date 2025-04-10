# ChatGPT Ingredient Recognition Analysis

This repository contains the code and results from our MSc group project, where we evaluated the performance of ChatGPT-4o in recognizing food ingredients from images. The analysis includes preprocessing of prediction data, performance evaluation, statistical testing, and ingredient-level error analysis.

## Project Overview

Our objective was to investigate how well ChatGPT-4o can predict food ingredients and whether its performance varies depending on image difficulty.

We structured the analysis into two main phases:

1. **Preprocessing & Normalization**
2. **Statistical Testing & Visualization**

---

## Notebooks

- `data_preprocessing.ipynb`:  
  Handles loading, cleaning, and normalizing the ground truth and ChatGPT-predicted ingredient labels. Applies a normalization map to ensure consistency for evaluation.

- `statistical_analysis.ipynb`:  
  Performs evaluation by computing precision, recall, and F1 score for each image. Includes statistical testing (Levene’s test, Kruskal-Wallis test, Dunn’s post hoc test) and visualization of results. Also contains an ingredient-level error analysis.

---

## Key Results

- **Performance varies with image difficulty:**  
  F1 scores were significantly lower for difficult images compared to easy and medium ones.

- **Statistical significance:**  
  Levene’s test indicated unequal variances, leading to the use of Kruskal-Wallis and Dunn’s test, which confirmed significant differences in performance.

- **Error patterns:**  
  ChatGPT frequently missed subtle ingredients like *onion*, *oil*, and *salt*, and overpredicted common ingredients like *cheese*, *beef*, and *sauce*.

---

## Visualizations

The repository includes plots illustrating:
- F1 score, precision, and recall distributions by difficulty
- Precision vs recall scatter plot
- Kruskal-Wallis and Dunn’s test results
- Most frequent false negatives and false positives

## Contact

If you have any questions or would like access to the image dataset used for prompting ChatGPT in these experiments, please feel free to contact us.

📧 [fouzia.shile@gmail.com]  
📁 Dataset access requests are welcome for academic or research purposes.

