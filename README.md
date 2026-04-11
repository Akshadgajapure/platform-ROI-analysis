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

---

## Files & Folder Structure

```
AB Testing/
├── main.ipynb                              # Main analysis notebook
├── global_ads_performance_dataset.csv      # Raw advertising performance dataset
├── DATASET.md                              # Dataset documentation
└── README.md                               # This file
```

---

## Dataset Description

**Dataset File**: [global_ads_performance_dataset.csv](global_ads_performance_dataset.csv)

**Documentation**: See [DATASET.md](DATASET.md) for detailed documentation on:
- Column descriptions
- Platform details (Google, Meta, TikTok)
- Industry categories
- Campaign types
- Geographic regions
- Data quality notes

---

## Getting Started

### Prerequisites
- Python 3.8+
- Jupyter Notebook or JupyterLab
- Required Libraries: pandas, numpy, scipy, matplotlib, seaborn

### Running the Analysis

1. Open the main notebook:
   ```bash
   jupyter notebook main.ipynb
   ```

2. Execute cells sequentially from top to bottom

3. The notebook will automatically load [global_ads_performance_dataset.csv](global_ads_performance_dataset.csv) and generate results

---

## Analysis Sections

The main analysis covers:

1. **Data Exploration** - Load dataset, check data types, missing values, platform distribution
2. **Descriptive Statistics** - Calculate mean, median, std dev for key metrics by platform
3. **Key Metrics Calculation** - Compute ROAS, CTR, and CPA for each campaign
4. **Statistical Testing** - Perform ANOVA to test platform differences (α = 0.05)
5. **Controlled Comparison** - Analyze platform performance within each campaign type
6. **Selection Bias Analysis** - Check campaign type distribution across platforms
7. **Visualizations** - Box plots, bar charts, and segmented performance views
8. **Recommendations** - Budget allocation strategy and next steps

---

## Key Metrics

### ROAS (Return on Ad Spend)
$$ROAS = \frac{Revenue}{Spend}$$
Higher is better. Target > 3.0x for profitability.

### CTR (Click-Through Rate)
$$CTR = \frac{Clicks}{Impressions} \times 100$$
Percentage of viewers who clicked. Indicates ad relevance.

### CPA (Cost Per Acquisition)
$$CPA = \frac{Spend}{Conversions}$$
Cost to acquire one customer. Lower is better.

---






## Key Takeaways

✅ **TikTok shows higher average ROAS** but differences shrink when controlling for campaign type  
✅ **Selection bias is significant** — high-performing platforms are allocated more favorable campaign types  
✅ **Budget allocation should prioritize campaign objectives first**, not platform choice  
✅ **Recommend controlled testing** with 10–15% budget before major reallocation  
✅ **Medium confidence level** — statistical signal is strong, but observational data limits causal inference  



