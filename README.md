# **RFM ANALYSIS** 
***>>> For further details, please refer to RFM_Analysis.ipynb <<<***
## **1. Goal**
To segment customers based on their purchasing behavior using the RFM framework and develop data-driven, actionable marketing strategies for each customer segment.

## **2. Key Results**
**Time range:** 2010-12-01 to 2011-12-09

To profile users, 3 key behavioral metrics are analyzed at the monthly level:
- Recency: Days since last order (DSLO)
- Frequency: Total orders
- Average Monthly Monetary (AMM): average monthly gmv
  <img width="1138" height="160" alt="image" src="https://github.com/user-attachments/assets/55afcd2d-32fe-4c83-92ba-246b1e9c9570" />

## **3. Method**
- **RFM Analysis** to quantify customer behavior.
- **Log transformation** to stabilize skewed distributions.
- **Feature scaling (Standardization)** to normalize variables before clustering.
- **Elbow Method & Silhouette Score** to determine the optimal number of clusters.
- **K-Means clustering** to categorize customers into distinct segments.
- **Cluster profiling & CRM lifecycle** to convert clusters into business-relevant lifecycle segments.
## **4. Main Steps**

- **Data Quality Check**: Assess missing values, duplicates, invalid records, and cancelled transactions, etc.
- **Data Cleaning**: Remove duplicates, exclude cancelled and invalid transactions.
- **Build RFM Table**: Calculate Recency, Frequency, and Monetary at customer level.
- **RFM Skewness Check**: Identify whether data is strong skewness in any RFM, to be well prepare before apply Kmean
- **Log Transformation & Scaling**
- **K-Means Clustering**: Use Elbow Method and Silhouette Score to select optimal K.
- **User Profiling & CRM Lifecycle**: Translate clusters into lifecycle segments: Early Life, Mature, Prevent Churn, Churn

## **5. Marketing Strategy Suggestion**
#### Early Life Objective: Help customers build a consistent shopping habit by encouraging more frequent purchases in the early stage.

- Double Day campaigns (e.g., 9.9, 10.10, 11.11) with attractive vouchers to make shopping feel exciting and rewarding.
- Run Payday promotions around salary periods to match customers's higher purchasing power.
- Provide reward for 1st-to-2nd and 2nd-to-3rd purchases to gently guide them toward repeat buying.
- Introduce daily check-in rewards (points, small vouchers, loyalty credits) to increase daily engagement.


#### Mature Objective: Maintain engagement and strengthen loyalty among these high-value users.
- Develop loyalty tiers or VIP programs to reward consistent engagement.
- Provide exclusive offers.
- Recommend premium or high-value products through upsell and cross-sell.
- Introduce daily check-in rewards (points, small vouchers, loyalty credits) or simple weekly missions to keep user retention.

#### Prevent Churn Objective: Re-engage and prevent customers from slipping into full inactivity.
- Use personalized push notifications or emails to bring them back
- Offer personalized comeback vouchers.
- Run re-engagement campaigns during Double Day or seasonal events.
- Provide tailored product recommendations based on their previous purchases.

#### Churn Objective: Reactivate selectively while maintaining marketing efficiency and cost control.
- Launch win-back campaigns with an attractive discount (but control cost)
- Use personalized push notifications or emails to bring them back
- Reintroduce best-selling or trending products with limited-time comeback offers.

## **6. Further Analysis - Golden Number Analysis**
**Goal:**
To identify the purchase milestone at which customers begin to form stable shopping habits, churn rate is analyzed across cumulative order counts.

The analysis aims to detect a significant drop in churn probability after a certain purchase threshold (aka 'Golden Number'), indicating behavioral stabilization and stronger retention patterns.

**Strategy:**

Once the Golden Number is identified, marketing efforts should focus on accelerating customers toward this milestone.
Campaigns and incentives can be tailored to encourage repeat purchases until customers reach this critical order count
