![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Assessment | Statistical Evaluation and Communication

## Overview

This final assessment brings together everything you have learned across the Statistics for Data Science module. You will perform an end-to-end analysis that spans correlation analysis, group comparisons, statistical visualization, and machine-learning metric evaluation with uncertainty quantification.

Real-world data projects rarely involve a single technique. Decision-makers need analysts who can choose the right method for each question, execute it correctly, and weave the results into a coherent narrative. This assessment mirrors that workflow: you will move from exploration to inference to evaluation, just as you would in a professional setting.

The assessment culminates in an evaluation memo that synthesizes your findings into a recommendation. This is where analytical skill meets communication skill — the combination that makes data professionals effective.

## Learning Goals

- Compute and interpret Pearson and Spearman correlations with appropriate significance tests
- Perform one-way ANOVA and post-hoc comparisons to evaluate group differences
- Create publication-quality statistical visualizations that support your narrative
- Use bootstrap resampling to construct confidence intervals for ML evaluation metrics
- Synthesize multiple analyses into a coherent evaluation memo with actionable recommendations

## Prerequisites

- Python 3.9+
- Libraries: pandas, numpy, scipy, statsmodels, scikit-learn, matplotlib, seaborn

```bash
pip install pandas numpy scipy statsmodels scikit-learn matplotlib seaborn
```

## Requirements

1. **Fork** the assessment repository to your GitHub account.
2. **Clone** your fork locally.
3. Work inside the Jupyter notebook named **`m3-13-assessment.ipynb`**.
4. Commit and push your work regularly.

## Tasks

### Task 1 — Correlation Analysis

1. Select at least three pairs of numeric variables and compute both Pearson and Spearman correlation coefficients.
2. Test each correlation for statistical significance and report p-values.
3. Create a correlation heatmap and at least two scatter plots with regression lines.
4. Discuss when Pearson vs. Spearman is more appropriate given the data's characteristics.

### Task 2 — Group Comparisons with ANOVA

1. Identify a categorical variable with three or more groups and a continuous outcome variable.
2. Check ANOVA assumptions (normality within groups, homogeneity of variance).
3. Perform a one-way ANOVA and report the F-statistic, p-value, and effect size (eta-squared).
4. If the ANOVA is significant, run Tukey's HSD post-hoc test and interpret pairwise differences.
5. If assumptions are violated, apply the Kruskal-Wallis alternative and compare results.

### Task 3 — Statistical Visualization

1. Create at least four publication-quality visualizations that support your analysis from Tasks 1–2.
2. Each visualization must include: a descriptive title, labeled axes, a legend (if applicable), and annotation of key statistical results (e.g., r-value on scatter plots, significance brackets on group comparisons).
3. Use color, layout, and design choices intentionally to guide the reader's attention.
4. Write a one-paragraph caption for each visualization explaining its message.

### Task 4 — Bootstrap Confidence Intervals for ML Metrics

1. Using a provided set of model predictions and true labels, compute accuracy, precision, recall, and F1-score.
2. Implement bootstrap resampling (at least 2 000 iterations) to construct 95% confidence intervals for each metric.
3. Visualize the bootstrap distributions and confidence intervals (e.g., histogram with shaded CI region).
4. Interpret the intervals: How certain can you be about the model's performance? Are any metrics unreliable given the sample size?

### Task 5 — Evaluation Memo

1. Write an evaluation memo (500–700 words) that synthesizes findings from Tasks 1–4.
2. Structure: Context → Key Findings → Limitations → Recommendations.
3. Address a hypothetical stakeholder who needs to decide whether to deploy or iterate on the model.
4. Reference specific statistical evidence (correlations, group differences, metric CIs) to support your recommendation.
5. Use clear, professional language accessible to a mixed technical/non-technical audience.

## Submission

### What to submit

- A completed Jupyter notebook (`m3-13-assessment.ipynb`) with all code, outputs, and markdown explanations.
- The evaluation memo can be included as a final markdown section in the notebook.

### Definition of done

- [ ] Correlation analysis includes Pearson, Spearman, significance tests, and visualizations
- [ ] ANOVA is performed with assumption checks, effect size, and post-hoc tests
- [ ] At least four publication-quality visualizations with captions are included
- [ ] Bootstrap CIs are computed for four ML metrics with distribution plots
- [ ] Evaluation memo is 500–700 words with clear structure and evidence-based recommendations
- [ ] All statistical results are interpreted in plain language alongside technical values
- [ ] Notebook runs top-to-bottom without errors

### How to submit

1. Stage and commit your changes:
   ```bash
   git add .
   git commit -m "Complete m3-13 assessment"
   ```
2. Push to your fork:
   ```bash
   git push origin main
   ```
3. Open a **Pull Request** from your fork to the original repository.
4. Paste the Pull Request URL into the Student Portal.

## Evaluation Criteria

| Criterion | Weight | Description |
|---|---|---|
| Correlation Analysis | 15% | Correct computation, appropriate method choice, and clear interpretation |
| ANOVA & Group Comparisons | 20% | Proper assumption checks, correct execution, and meaningful post-hoc analysis |
| Statistical Visualization | 20% | Publication-quality charts with annotations, captions, and intentional design |
| Bootstrap ML Metrics | 20% | Correct implementation, clear visualization, and thoughtful interpretation |
| Evaluation Memo | 20% | Well-structured, evidence-based, and accessible to mixed audiences |
| Code Quality | 5% | Clean, well-organized notebook that runs without errors |
