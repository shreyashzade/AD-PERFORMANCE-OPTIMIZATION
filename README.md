# AD-PERFORMANCE-OPTIMIZATION

1. **Advertisement Campaign Evaluation**: Evaluating a client's current advertisement campaign across different platforms and providing strategic solutions to increase return on investment (ROI). 

## Problem Statement : Advertisement Campaign Evaluation
The primary objective is to maximize the ROI for our client's advertising campaigns. The client has conducted two ad campaigns, one on Facebook and the other on AdWords. The task is to determine which platform yields better results in terms of clicks, conversions, and overall cost-effectiveness.

### Key Questions
- Which ad platform is more effective in terms of conversions, clicks, and overall cost-effectiveness?
- What is the cost-per-click (CPC) trend over a 12-month period?
- Is there a long-term equilibrium relationship between advertising spend and conversion rates?

### Expected Outcomes
- Identification of the more effective ad platform.
- Insights into cost-per-click trends.
- Establishing a stable, long-term relationship between advertising spend and conversion rates, guiding strategic budget allocations.

## Dataset Description
The dataset includes performance metrics from ten separate ad campaigns conducted throughout 2023. The key features include:
- **Date**: The date corresponding to each row of campaign data.
- **AdViews**: Number of times the ad was viewed.
- **AdClicks**: Number of clicks received on the ad.
- **AdConversions**: Number of conversions resulting from the ad.
- **Cost per Ad**: Cost associated with running the ad campaign.
- **Click-Through Rate (CTR)**: Ratio of clicks to views.
- **Conversion Rate**: Ratio of conversions to clicks.
- **Cost per Click (CPC)**: Average cost incurred per click on the ad.

## Methodology

1. **Data Overview**: Analyzed the data using Pandas functions (head, info, describe, etc.), adjusting data types as needed.
2. **Distribution Analysis**: Plotted distribution curves to visualize and identify patterns in the data.
3. **Conversion Frequency Analysis**: Compared conversion frequencies by creating conversion categories and merging data frames for different ad campaigns.
4. **Correlation Analysis**: Calculated the Pearson Correlation Coefficient to analyze the relationship between the number of clicks and sales.
5. **Hypothesis Testing**: Used hypothesis testing to compare the effectiveness of Facebook ads vs. AdWords ads.
6. **Regression Analysis**: Performed regression analysis using XGBoost and Linear Regression to predict conversions based on ad clicks.
7. **Weekly & Monthly Metrics Analysis**: Analyzed Facebook campaign’s weekly and monthly conversion metrics.
8. **CPC Trend Analysis**: Analyzed the Cost Per Conversion (CPC) trend over time.
9. **Equilibrium Relationship Analysis**: Examined the long-term equilibrium relationship between advertising spend and conversion rates.

## Key Findings

### Distribution Analysis
- The histograms suggest a relatively symmetrical distribution of clicks and conversions across all campaigns.

### Conversion Frequency
- Facebook had more frequent higher conversion days compared to AdWords, which had mostly low to moderate conversion days.

### Correlation Analysis
- **Facebook**: Strong positive correlation (0.87) between clicks and sales.
- **AdWords**: Moderate positive correlation (0.45) between clicks and sales.

### Hypothesis Testing
- The mean number of conversions from Facebook ads (11.74) is substantially higher than from AdWords ads (5.98).
- The p-value (9.35e-134) strongly supports the hypothesis that Facebook ads are more effective in generating conversions.

### Regression Analysis
- The Linear Regression model had a good predictive power with an R² score of 76.35%, indicating that it can effectively predict Facebook ad conversions based on clicks.

### Weekly & Monthly Metrics Analysis
- Mondays and Tuesdays had the highest conversion rates, while certain months (e.g., February, April, May, June, August, and November) showed declines.

### CPC Trend Analysis
- CPC values fluctuated but remained relatively stable, with May and November having the lowest CPC values.

### Equilibrium Relationship Analysis
- A long-term equilibrium relationship was found between advertising spend and conversions, suggesting that businesses can optimize their advertising strategies based on this relationship.

## Conclusion
Facebook advertising is more effective in driving conversions compared to AdWords. Businesses should consider reallocating resources towards Facebook ads to maximize ROI. Additionally, the developed web analytics tool enables clients to gain insights into user behavior, facilitating customer-oriented decision-making.

## Acknowledgement
Special thanks to the data science and analytics team for their support and contributions to this project.

## Resources Used
- Python (Pandas, NumPy, Scikit-learn, XGBoost)
- Data visualization libraries (Matplotlib, Seaborn)
- Statistical tools for hypothesis testing and regression analysis

