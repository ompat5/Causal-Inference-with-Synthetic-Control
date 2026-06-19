# Causal-Inference-Analysis
## Project Overview
This project evaluates the causal impact of a regional billboard campaign on customer deposits in Porto Alegre. Since randomized A/B testing was not feasible for an offline city-level intervention, the notebook uses a Difference-in-Differences design to estimate the treatment effect by comparing Porto Alegre against Florianopolis across pre- and post-campaign periods.

## Causal Framework
The analysis applies core causal inference concepts, including:
- Difference-in-Differences (DiD) to estimate treatment lift from panel-style regional data.
- Counterfactual reasoning to compare observed post-treatment outcomes against expected outcomes without intervention.
- Interaction-term regression to recover the DiD estimator and quantify the campaign effect in a statistical model.

## Data and Methodology
The dataset contains deposit observations across two cities and two time periods: Porto Alegre as the treatment group, Florianopolis as the control group, May as the pre-intervention period, and July as the post-intervention period. The statistical approach includes:
- Before-after and treated-vs-control comparisons to show why naive estimators are biased.
- Manual computation of the Difference-in-Differences estimator
- Ordinary Least Squares regression with time, treatment, and interaction terms to estimate the effect and report standard errors, p-values, and confidence intervals.
