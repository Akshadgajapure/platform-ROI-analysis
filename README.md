# 📊 Advertising Platform Performance Analysis

This project analyzes the performance of **Google Ads, Meta Ads, and TikTok Ads** using statistical analysis to determine whether differences in advertising performance are genuine or influenced by selection bias.

## 🎯 Objective
- Compare advertising platform performance using **ROAS, CTR, and CPA**
- Validate differences using statistical tests
- Detect selection bias in campaign allocation
- Provide actionable business recommendations

## 🛠️ Tech Stack
- Python
- Pandas
- NumPy
- SciPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## 📈 Statistical Methods
- Descriptive Statistics
- Bootstrap Confidence Intervals
- One-Way ANOVA
- Tukey HSD
- Effect Size (η² & Cohen's d)
- Selection Bias Analysis

## 📌 Key Findings
- TikTok Ads achieved the highest raw ROAS (9.54x vs Google's 4.11x).
- Platform differences were statistically significant (**ANOVA, p < 0.001**).
- Platform explained **10.7%** of ROAS variation (η² = 0.107, large effect).
- Campaign type distribution was uneven across platforms (a potential selection bias risk).
- After controlling for campaign type, the TikTok–Google ROAS gap was **essentially unchanged** (+5.43x raw vs +5.46x controlled) — meaning campaign-type mix does **not** explain TikTok's advantage in this dataset, and the effect appears genuine rather than a bias artifact.

## 💡 Business Recommendation
Campaign-type mix was checked as a likely confounder and ruled out — TikTok's advantage held up within every campaign type individually. That said, this remains observational data with other unchecked variables (country, industry, seasonality), so budget shifts should still be validated with a controlled A/B test (10–15% of budget, ~4 weeks) before fully reallocating spend, and results should be revisited quarterly as platform dynamics change.

---
**Skills Demonstrated:** Data Analysis • Statistical Inference • Hypothesis Testing • Confounding & Bias Detection • Data Visualization • Business Analytics
