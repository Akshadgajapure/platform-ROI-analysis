#  Multi-Platform Advertising Performance Analysis

## Problem

Which advertising platform (Google, Meta, TikTok) delivers the best ROI?

## Key Insight

What looks like platform performance is largely **campaign type + intent matching**, not just platform superiority.

## Approach

* Exploratory analysis (ROAS, CTR, CPA)
* ANOVA to test statistical differences
* Controlled comparison (within campaign type)
* Bias analysis (selection bias check)

## Key Findings

* TikTok shows higher average ROAS
* BUT differences shrink when controlling for campaign type
* Indicates **selection bias plays a major role**

## Recommendation

* Do NOT blindly shift budget
* Allocate by **campaign objective first**
* Run controlled test (10–15% budget) before scaling

## Confidence Level

Medium — statistical signal is strong, but causal inference is limited due to observational data

## Tools Used

Python, Pandas, NumPy, SciPy, Matplotlib, Seaborn
