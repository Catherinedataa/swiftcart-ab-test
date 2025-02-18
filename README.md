# SwiftCart A/B Testing

## Overview

SwiftCart is an e-commerce platform aiming to enhance user experience and increase online sales. This project focuses on an A/B test conducted to evaluate whether a redesigned checkout process improves conversion rates.

The company implemented a new, streamlined checkout process for a subset of users (Test Group) while keeping the existing checkout for the Control Group. The goal was to determine if the new process led to a higher conversion rate by reducing friction in completing purchases.

Below is the overview page from the power bi dashboard
![overview](https://github.com/user-attachments/assets/a6a4350c-79a7-43bb-bb65-f0bd24eddb41)


## Insights & Recommendations

Insights and recommendations are structured around the following key areas:

 **Conversion Rate Impact**  Did the new checkout increase conversions?
 
 **Statistical Significance**  Were the results meaningful, or due to random chance?
 
 **Business Implications**  What does this mean for SwiftCart’s future optimizations?

  The  interactive Power BI Dashboard can be accessed here: [link](https://github.com/Catherinedataa/swiftcart-ab-test/blob/main/abtestingdashboard.pbix)
  
  The Jupyter notebook can be can be accessed here: [link](https://github.com/Catherinedataa/swiftcart-ab-test/blob/main/abtesting.ipynb)

  ##  Data Structure and Initial Checks
The dataset used for this A/B test was collected from SwiftCart’s marketing campaigns, focusing on performance metrics like spend, impressions, website interactions, and conversions. The data spans from 1st April 2024 to 30th June 2024, capturing performance across various campaigns and user interactions. These features were further analyzed to assess the impact of the new checkout process on conversion rates.
Below is a brief description of the structure of the dataset used for A/B testing:

campaign_name	: Describes the A/B test group: 'Control' or 'Test																							

date: Date of the campaign																							

spend_usd: Amount of money spent in USD for the campaign																							

impressions:	Number of impressions generated by the campaign																							

reach: Total reach or number of unique users exposed to the campaign																							

website_clicks: Number of clicks on the website from the campaign																							

searches: Number of searches initiated from the campaign																							
add_to_cart: Number of times content was viewed during the campaign																							
purchases: Number of users who added items to their cart during the campaign																							
conversion_rate: Number of purchases completed during the campaign																							
cost_per_conversion: Cost per conversion calculated from total spend divided by purcha

### Key Metrics & Findings

After running a Z-test, the results showed:

 **Control Group Conversion Rate:** 5.76% (95% CI: 5.72% - 5.79%)
 
 **Test Group Conversion Rate:** 6.49% (95% CI: 6.46% - 6.53%)
 
 **Lift in Conversion Rate:** +12.81%
 
 **Z-Statistic:** 31.63
 
 **P-Value:** 6.21e-220 
 
 **Cohen’s h:** 0.0308
 
 **Power:** 1.000 (indicating high confidence in detecting a real effect)

## Conclusion & Business Implications

The new checkout process significantly increased conversions, with a 12.81% uplift compared to the old process. Given the low p-value (6.21e-220), we can confidently say this result is not due to random chance.

### Business Impact:

**Improved Conversion Rate:** A 12.81% increase in conversions means that more users are successfully completing the checkout process. This leads to more successful transactions, which translates into increased sales volume. 

**User Experience Enhancement:** The new checkout design reduces friction, making it easier for users to complete purchases. This likely improves customer satisfaction and could lead to higher retention rates, as customers prefer smoother and faster processes.  

**Scalability Considerations:** Given the statistically significant improvements, the new checkout process should be implemented site-wide. This offers the potential for further optimization with minor adjustments and enhancements over time, ensuring that SwiftCart stays competitive and continues to meet the evolving needs of customers.

### Next Steps:

  **Further A/B Tests:** Explore additional user-centric optimizations, such as One-click checkout to  test if simplifying the process further boosts conversions and User Segmentation to test different checkout processes for distinct user segments for example first-time visitors vs. returning users.
        
**Cost-Benefit Analysis:** Conduct a detailed financial analysis to ensure the long-term profitability of the new checkout process and assess the development and implementation costs against the projected revenue increase from higher conversions.
Factor in scalability considerations to ensure that future enhancements are cost-effective and sustainable as the user base grows.

**Full Rollout of New Checkout Process:** Deploy the new checkout system to all users on the platform. Ensure the rollout is phased to monitor its impact closely.
Key Metrics to Monitor: Track the conversion rate, abandonment rate and user satisfaction post-rollout. These can provide further insights into whether the new process continues to deliver improvements.


