# Global Ads Performance Dataset Documentation

## Overview

The **Global Ads Performance Dataset** contains comprehensive advertising metrics across three major advertising platforms: **Google Ads**, **TikTok Ads**, and **Meta Ads**. This dataset enables comparative analysis of advertising effectiveness across different industries, campaign types, and geographic regions.

---

## Dataset Summary

- **File Name**: `global_ads_performance_dataset.csv`
- **Total Records**: 200+ campaign performance entries
- **Platforms**: 3 (Google Ads, TikTok Ads, Meta Ads)
- **Industries**: 5 (Fintech, EdTech, Healthcare, E-commerce, SaaS)
- **Campaign Types**: 4 (Search, Video, Shopping, Display)
- **Geographic Coverage**: 5 countries (USA, UK, Canada, Germany, UAE)
- **Time Period**: Multiple dates spanning 2024

---

## Column Descriptions

### Core Identifiers

| Column | Type | Description |
|--------|------|-------------|
| `date` | Date | Campaign execution date (YYYY-MM-DD format) |
| `platform` | Categorical | Advertising platform (Google Ads / TikTok Ads / Meta Ads) |
| `campaign_type` | Categorical | Type of campaign (Search / Video / Shopping / Display) |
| `industry` | Categorical | Industry vertical (Fintech / EdTech / Healthcare / E-commerce / SaaS) |
| `country` | Categorical | Geographic location (USA / UK / Canada / Germany / UAE) |

### Traffic & Engagement Metrics

| Column | Type | Unit | Description |
|--------|------|------|-------------|
| `impressions` | Integer | Count | Number of times ads were shown to users |
| `clicks` | Integer | Count | Number of user clicks on advertisements |
| `CTR` | Float | Percentage | Click-Through Rate = (Clicks / Impressions) × 100 |

### Cost Metrics

| Column | Type | Unit | Description |
|--------|------|------|-------------|
| `ad_spend` | Float | USD | Total advertising expenditure for the day |
| `CPC` | Float | USD | Cost-Per-Click = (Ad Spend / Clicks) |
| `CPA` | Float | USD | Cost-Per-Acquisition = (Ad Spend / Conversions) |

### Conversion & Revenue Metrics

| Column | Type | Unit | Description |
|--------|------|------|-------------|
| `conversions` | Integer | Count | Number of successful conversions (purchases/sign-ups/leads) |
| `revenue` | Float | USD | Total revenue generated from conversions |
| `ROAS` | Float | Ratio | Return on Advertising Spend = (Revenue / Ad Spend) |

---

## Platform Details

### 1. Google Ads
- **Type**: Search and Shopping focused advertising
- **Best For**: High intent users actively searching for products/services
- **Campaign Types**: Primarily Search, Shopping, Display
- **Key Strength**: Direct response and conversion optimization

### 2. TikTok Ads
- **Type**: Video and social media advertising
- **Best For**: Brand awareness and younger demographics (Gen Z)
- **Campaign Types**: Primarily Video, Shopping, Search
- **Key Strength**: High engagement and viral potential

### 3. Meta Ads
- **Type**: Social media advertising (Facebook/Instagram)
- **Best For**: Interest/behavior targeting and retargeting
- **Campaign Types**: Video, Display, and Shopping
- **Key Strength**: Detailed audience segmentation

---

## Industries Covered

| Industry | Focus | Target |
|----------|-------|--------|
| **Fintech** | Financial Services | B2C Financial Solutions |
| **EdTech** | Education Technology | Online Learning Platforms |
| **Healthcare** | Health & Wellness | Medical Services & Products |
| **E-commerce** | Online Retail | Direct-to-Consumer Sales |
| **SaaS** | Software Services | B2B Software Solutions |

---

## Campaign Types

| Type | Description | Best For |
|------|-------------|----------|
| **Search** | Text ads in search results | High-intent keywords |
| **Video** | Video advertisements | Brand awareness & engagement |
| **Shopping** | Product ads with images | E-commerce & retail |
| **Display** | Graphic ads on partner sites | Retargeting & awareness |

---

## Geographic Regions

| Country | Region | Notes |
|---------|--------|-------|
| **USA** | North America | Largest market, diverse industries |
| **UK** | Europe | Established markets, GDPR compliance |
| **Canada** | North America | Bilingual market (EN/FR) |
| **Germany** | Europe | Strong B2B presence, privacy-focused |
| **UAE** | Middle East | Growing fintech & e-commerce sector |

---

## Key Performance Indicators (KPIs)

### Primary Metrics

1. **ROAS (Return on Advertising Spend)**
   - Formula: Revenue ÷ Ad Spend
   - Target: > 3.0x (3x return for every $1 spent)
   - Indicates overall campaign profitability

2. **CPA (Cost-Per-Acquisition)**
   - Formula: Ad Spend ÷ Conversions
   - Target: Lower is better
   - Critical for understanding acquisition efficiency

3. **CTR (Click-Through Rate)**
   - Formula: (Clicks ÷ Impressions) × 100
   - Average Range: 0.5% - 10% depending on platform
   - Indicates ad relevance and appeal

### Secondary Metrics

4. **CPC (Cost-Per-Click)**
   - Formula: Ad Spend ÷ Clicks
   - Indicates bidding efficiency
   - Varies by platform and competition

5. **Conversion Count**
   - Direct measure of campaign success
   - Used to calculate CPA and ROAS

6. **Impressions**
   - Total ad exposures
   - Indicates reach and visibility

---

## Data Quality Notes

- **No Missing Values**: All records are complete
- **Data Types**: Properly formatted for analysis
- **Value Ranges**: 
  - CTR: 0.01% - 0.95% (realistic ranges)
  - ROAS: 0.39x - 34.82x (varies significantly)
  - CPA: $7.66 - $134.74 USD

---

## Analysis Recommendations

### 1. Comparative Analysis
- Compare ROAS across platforms to identify top performer
- Analyze CPA by industry to find cost-effective segments
- Evaluate CTR to assess creative effectiveness

### 2. Segmentation Analysis
- Performance by industry → find best platform per vertical
- Performance by campaign type → optimize creative strategy
- Geographic performance → adjust regional budgets

### 3. Statistical Testing
- ANOVA to test significant differences between platforms
- T-tests for platform pairs comparison
- Correlation analysis between metrics

### 4. Optimization Opportunities
- Identify high-ROAS combinations (platform + industry + campaign type)
- Flag underperforming segments for optimization
- Monitor seasonal trends by date

---

## Use Cases

1. **Budget Allocation**: Determine optimal platform spending distribution
2. **Campaign Planning**: Select best platform for specific industry/type
3. **Performance Benchmarking**: Compare actual vs. industry standards
4. **A/B Testing**: Validate hypothesis about platform effectiveness
5. **Regional Strategy**: Optimize campaigns by geographic market

---

## Additional Notes

- Data spans multiple months in 2024
- Each record represents one day's campaign performance
- Multiple records per platform indicate daily tracking
- Revenue values represent conversions × average order value
- All financial values are in USD

---

**Last Updated**: April 2, 2026  
**Data Provider**: Marketing Analytics Team  
**For Questions**: Contact analytics@company.com
