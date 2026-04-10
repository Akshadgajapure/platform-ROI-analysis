# Clean A/B Testing: E-Commerce Checkout Optimization

## Project Overview

This is a **true randomized A/B test** demonstrating proper experimental design. We test a simplified checkout flow against the current experience and measure impact on conversion rates.

### Experiment Setup
- **Variant A (Control):** Current checkout flow  
- **Variant B (Treatment):** Simplified checkout (fewer fields, faster process)
- **Sample Size:** 500 users per variant (1,000 total)
- **Randomization:** Users randomly assigned at session start
- **Primary Metric:** Conversion rate (binary: converted or not)
- **Secondary Metrics:** Session duration, order value

### Key Differences from Observational Analysis

| Aspect | This Project | Previous Project |
|--------|------------|-----------------|
| **Design** | Randomized experiment (RCT) | Observational data |
| **Causation** | ✓ Can infer causation | ✗ Correlation only |
| **Confounding** | ✓ Randomization controls bias | ✗ Selection/measurement bias |
| **Familiarity** | ✓ Easy to explain to stakeholders | ✓ Closer to real business scenarios |
| **What it shows** | "What happens if we change X?" | "Which X is working best?" |

---

## Analysis Methodology

### 1. Randomization Check
Verify both groups balanced on key characteristics (session duration)

### 2. Hypothesis Test
**H₀:** Variant A and Variant B have equal conversion rates  
**H₁:** Variant B has higher conversion rate (one-tailed test)

Based on:
- Chi-squared test (categorical outcome)
- Confidence interval approach
- Statistical power consideration

### 3. Business Impact
- **Absolute conversion lift:** % point difference
- **Relative conversion lift:** % improvement
- **Statistical significance:** p-value < 0.05
- **Practical significance:** Is the improvement worth switching?

### 4. Sample Size Justification
With 500 per group, we have 80%+ power to detect 4% relative improvement (baseline 18% → 18.7%)

---

## Business Recommendation Framework

| Scenario | Action |
|----------|--------|
| **p < 0.05 + Practical lift > 2%** | ✅ Launch Variant B → Expected ROI positive |
| **p < 0.05 + Practical lift < 1%** | ⚠️ Statistically significant but small impact → Consider other priorities |
| **p ≥ 0.05** | ❌ No significant difference → Keep current variant |
| **Confounded results?** | Extend test, add cohort analysis |

---

## Files
- `ecommerce_ab_test.csv` - Experiment data (1,000 sessions)
- `ab_analysis.ipynb` - Full notebook with statistical tests
- `README.md` - This file

## Interview Talking Points

When discussing this project:

1. **What makes it a true A/B test?**  
   "Random assignment of users at session start eliminates selection bias. Every user had 50/50 chance of seeing Variant A or B."

2. **How do you measure success?**  
   "Primary metric is conversion rate. Secondary metrics show why the change works (session duration suggests reduced friction)."

3. **What if the test was inconclusive?**  
   "Could extend sample size. Could also segment by user cohort—maybe works differently for mobile vs desktop. Or analyze Session duration as mediator."

4. **Why not just implement if p < 0.05?**  
   "Statistical significance ≠ business significance. A 0.2% lift might be significant but not worth engineering effort. Also need to consider other factors."

---

## Next Steps
- Compare results to observational analysis (previous project)  
- Discuss why causal insights from A/B tests are more reliable
- Show how to combine experimental + observational approaches
