# Optimizing User Engagement: A/B Testing with Digital Media Data

## Vision
A/B Testing is a powerful method for making data-driven decisions. It helps compare different versions of a feature or product to understand their impact on user behavior. This project demonstrates how statistical methods like A/B Testing and hypothesis testing can be used to make informed business decisions.

For more details on A/B Testing, refer to [this Harvard Business Review article](https://hbr.org/2017/06/a-refresher-on-ab-testing).

## Objectives
Using data from 20,000 customers, the project aims to:
- Analyze whether the user engagement in the treatment group (ad group) significantly exceeds that of the control group (PSA).
- Apply statistical testing methods to determine whether the observed results justify replacing PSA with advertising.

## Dataset
The dataset for this project is sourced from Kaggle and can be found [here](https://www.kaggle.com/datasets/).

## Methodology
1. **Exploratory Data Analysis (EDA)**:
   - Visualize the distribution of groups using `sns.countplot`.
   - Analyze user conversion rates across groups.

2. **Statistical Testing**:
   - Define hypotheses:
     - **Null Hypothesis (H₀)**: No difference in conversion rates between the control and treatment groups.
     - **Alternative Hypothesis (H₁)**: A significant difference exists between the conversion rates.
   - Calculate:
     - Conversion rates with confidence intervals.
     - Lift (percent improvement in conversion rate).
     - p-value using the Z-test.
     - Effect size (Cohen's h).

3. **Result Interpretation**:
   - Determine statistical and practical significance.
   - Provide actionable insights.

## Key Findings
- **Control Conversion Rate**: 3.23% (95% CI: 2.84% - 3.62%)
- **Treatment Conversion Rate**: 6.66% (95% CI: 6.22% - 7.11%)
- **Lift**: 106.01%
- **p-value**: ~0 (statistically significant)
- **Effect Size (Cohen's h)**: 0.16 (modest improvement)

The treatment group significantly outperformed the control group in conversion rates. While the effect size indicates a modest improvement, the results are statistically significant, providing a strong case for implementing the advertising strategy.

## Technologies Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Statsmodels

## How to Run
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`.
3. Run the Jupyter notebook: `jupyter notebook code.ipynb`.

## Acknowledgments
Special thanks to Kaggle for providing the dataset and to [Harvard Business Review](https://hbr.org) for A/B Testing insights.


