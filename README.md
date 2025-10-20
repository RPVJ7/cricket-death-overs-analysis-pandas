# 🏏 MS Dhoni – Death Overs Effectiveness Analysis

This project evaluates whether MS Dhoni remains effective in the finishing role — batting during overs 17–20 in T20 cricket — by comparing his key batting metrics against other players who have faced at least 100 balls in the same phase.

It demonstrates data-driven performance evaluation, metric definition, and comparative analysis using cricket data.

# ✨ Project Overview

The notebook analyzes ball-by-ball T20/IPL data to answer a focused question:
Is MS Dhoni still effective at the death (overs 17–20)?

# Context
Dhoni has built his career around finishing matches in pressure situations. As a lower-order batsman (usually positions 6–8), he often faces fewer balls — but in the most crucial phase of the innings.

# Objective
To evaluate Dhoni’s current finishing ability by comparing him with other batsmen who have faced a statistically meaningful number of balls (≥100) during overs 17–20.

# 📊 Key Metrics

Three performance indicators are computed to measure finishing effectiveness:

-  Strike Rate (SR) - 	100 × (Runs Scored / Balls Faced)	Ability to score quickly
-  Boundary %	- 100 × (Balls Hit for 4s or 6s / Balls Faced)	Power hitting capability
-  Dot Ball %	- 100 × (Balls with No Runs / Balls Faced)	Ability to rotate strike and handle pressure

Together, these metrics provide a comprehensive picture of a finisher’s efficiency and impact in the death overs.

# 🧠 Methodology

# 1. Data Preparation

Load and inspect IPL/T20 batting data up to 2021.
Validate player names, over numbers, and match context.
Focus exclusively on deliveries from overs 17–20.

# 2. Cohort Definition

Retain only batsmen with ≥100 balls faced in death overs to ensure meaningful sample sizes.
Aggregate total runs, boundaries, and dot balls for each batsman.

# 3. Metric Calculation

Compute Strike Rate, Boundary %, and Dot Ball % per batsman.
Store the metrics in a summary dataframe for comparison.

# 4. Peer Comparison

Compare Dhoni’s metrics with the rest of the cohort.
Rank all batsmen and compute percentile standings for each metric.
Visualize Dhoni’s position within the top finishers’ distribution.

# 5. Visualization

Scatter Plot: Strike Rate vs Dot Ball % (trade-off between aggression and rotation).
Bar Charts: Dhoni’s metrics vs cohort average.
Density/Box Plots: Dhoni’s standing within overall metric distributions.

# 📈 Results Summary

# Baseline Evaluation (All Features):
Initial strike-rate-based comparison showed modest results when using all available features directly.

# Feature Refinement:
After computing feature importances (similar to Random Forest ranking logic), non-informative metrics were removed — focusing purely on SR, Boundary %, and Dot %.
This improved interpretability and accuracy of comparisons.

# Final Findings:

  - Dhoni consistently ranks within the top 7 batsmen on Strike Rate and Boundary %.
  - His Dot Ball % remains among the best, showing efficient strike rotation.
  - Overall, Dhoni achieves approximately 70–75% effectiveness when benchmarked against the best finishers (top percentile group).

# Interpretation:

Dhoni continues to perform at a high-impact level in death overs, maintaining a strong balance of boundary frequency and pressure control — key attributes for a finisher.
While age has slightly affected raw strike rate, his game awareness and consistency remain elite.


# 🧰 Tools and Libraries

  - Python (Pandas, NumPy, Matplotlib, Seaborn)
  - Jupyter Notebook for data exploration and visualization
  - Statistical reasoning for cohort and percentile comparisons

# ▶️ Running the Notebook

  1.  Open the notebook in Jupyter Notebook or JupyterLab.
  2.  Execute each cell in sequence:
  3.  Load and clean the dataset
  4.  Filter overs 17–20
  5.  Compute key metrics
  6.  Compare Dhoni’s metrics with peers
  7.  Visualize results and interpret performance
  8.  Review the outputs in the summary and visualization sections for interpretation.

#  🧑‍💻 Skills Demonstrated

  - Sports analytics and cricket-specific data modeling
  - Metric definition and standardization
  - Cohort-based statistical comparison
  - Visualization of performance distributions
  - Reproducible data storytelling using Jupyter

# 🏁 Summary

This analysis demonstrates how data-driven performance evaluation can answer nuanced sporting questions.
By defining clear metrics, building a valid comparison group, and interpreting the results with context, the project concludes that MS Dhoni remains among the most effective finishers in modern T20 cricket — a testament to his adaptability, experience, and skill.
