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

## Dataset Description

See **DATASET.md** for detailed documentation on:
- Column descriptions
- Platform details
- Industry categories
- Campaign types
- Geographic regions
- Data quality notes

---

## Methodology

### Statistical Approach
- **Hypothesis Testing**: ANOVA with α = 0.05 significance level
- **Descriptive Statistics**: Mean, median, standard deviation analysis
- **Comparative Analysis**: Platform-to-platform comparisons
- **Segmentation**: Industry, campaign type, and geographic breakdowns

### Limitations
- Analysis based on 2024 data only
- Results may vary with seasonal changes
- External factors not captured in dataset
- Requires continuous monitoring for trend detection

---

## Next Steps

1. **Export Results**: Share key findings with stakeholders
2. **Implement Changes**: Adjust budgets based on recommendations
3. **Monitor KPIs**: Track performance post-implementation
4. **Iterate**: Run new tests and update analysis quarterly
5. **Expand Analysis**: Add more platforms, industries, or metrics

---

## Contact & Support

For questions or issues with this analysis:
- Review the notebook comments for methodology details
- Check DATASET.md for data specifications
- Verify data freshness before re-running analysis

---

## Changelog

| Date | Version | Changes |
|------|---------|---------|
| 2026-04-02 | 1.0 | Initial analysis complete |

---

**Created**: April 2, 2026  
**Last Updated**: April 2, 2026  
**Status**: Ready for implementation
