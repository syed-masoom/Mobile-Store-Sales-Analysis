# 📱 Mobile E-Store Sales Dashboard | Power BI Business Intelligence Project

<p align="center">
  <img src="https://img.shields.io/badge/Tool-Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" />
  <img src="https://img.shields.io/badge/Analysis-Sales%20%26%20Customer%20Insights-2EA44F?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Focus-Mid--Range%20Phones-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" />
</p>

<p align="center">
  <b>Power BI dashboard project analyzing mobile sales performance, customer purchase behavior, payment preferences, and marketing opportunities for mid-range smartphones.</b>
</p>

---

## 🚀 Project Overview

This project is based on a business scenario for a **Mobile E-Store** that wants to improve conversion rates for **mid-range smartphones**, especially brands and models such as Realme, Pixel, and similar devices.

The main business question was:

> **Why do customers buy mid-range phones, and what should the business highlight in campaigns: gaming, performance, features, price, or payment offers?**

To answer this, I built an interactive **Power BI Sales Dashboard** that helps analyze revenue, profit, orders, ratings, purchase reasons, income-level behavior, payment preferences, and top-selling mid-range phone models.

---

## 🎯 Business Objective

The objective of this analysis was to help the business understand:

- Which purchase reasons are most strongly linked with mobile phone sales.
- Whether customer income levels influence buying motivation.
- Which mid-range phone models perform best in terms of revenue and order volume.
- Whether higher-rated products share common behavioral patterns.
- Which marketing strategies can increase conversion rates for mid-range phones.

---

## 🧩 Key Business Questions

This dashboard answers the following questions:

1. **What is the overall sales performance of the mobile store?**
2. **How much revenue and profit comes from mid-range phones?**
3. **What are the top purchase reasons for mid-range customers?**
4. **Which payment methods are most preferred by customers?**
5. **Do low, medium, and high-income customers buy for different reasons?**
6. **Which mid-range phone models are best-selling?**
7. **What marketing actions should the business take next?**

---

## 🗂️ Dataset & Data Source

The dataset was created using an AI-generated business dataset based on a mobile store sales scenario. After generating the dataset, I performed multiple cleaning and preparation steps before building the dashboard.

### Data Preparation Workflow

1. Generated a structured mobile sales dataset.
2. Imported the dataset into Excel for initial validation and cleanup.
3. Cleaned missing, inconsistent, and formatting-related issues.
4. Combined order-level and customer-level information.
5. Used Excel functions such as:
   - `VLOOKUP`
   - `XLOOKUP`
   - `SUMIF`
   - Basic calculated fields
6. Exported the final cleaned dataset.
7. Loaded the dataset into Power BI for reporting and visualization.

---

## 🛠️ Tools & Skills Used

| Area | Tools / Techniques |
|---|---|
| Data Cleaning | Excel, Power Query |
| Data Transformation | Power BI Power Query Editor |
| Data Modeling | Power BI Data Model |
| Calculated Fields | DAX |
| Visualization | Power BI Dashboard |
| Business Analysis | KPI Tracking, Sales Analysis, Customer Segmentation |
| Storytelling | Insight Generation, Marketing Recommendations |

---

## ⚙️ Power BI Data Preparation

After loading the cleaned dataset into Power BI, I performed further transformation and modeling.

### Key Power BI Preparation Steps

- Removed unnecessary columns.
- Checked data types for numeric, categorical, and date fields.
- Created calculated columns for better segmentation.
- Built KPI measures for revenue, orders, profit, and average rating.
- Created business-friendly categories for dashboard filtering.

### Calculated Columns Created

```DAX
Price Range = 
SWITCH(
    TRUE(),
    Sales[Price] <= 20000, "Affordable",
    Sales[Price] <= 40000, "Mid-Range",
    "Expensive"
)
```

```DAX
Rating Category =
SWITCH(
    TRUE(),
    Sales[Rating] >= 4.2, "Satisfied",
    Sales[Rating] >= 3.5, "Good",
    "Not Satisfied"
)
```

---

## 📊 Dashboard Preview

<p align="center">
  <img src="https://raw.githubusercontent.com/syed-masoom/Sales-Dashboard-Power-Bi/refs/heads/main/Mobile%20Sales%20Dashboard.png" width="100%" alt="Mobile Sales Power BI Dashboard" />
</p>

---

## 📌 Dashboard Features

The dashboard includes multiple interactive visuals designed to support business decision-making.

### Main Dashboard Elements

- **KPI Cards**
  - Total Revenue
  - Total Orders
  - Average Rating
  - Total Profit

- **Sales by Purchase Reason**
  - Shows why customers are buying phones.

- **Sales by Payment Method**
  - Identifies preferred payment behavior.

- **Sales by Income Level and Purchase Reason**
  - Compares buying motivation across income groups.

- **Revenue by Phone Model**
  - Highlights top-performing mobile models.

- **Interactive Slicers**
  - Price Range Filter
  - Rating Category Filter

---

## 📈 Overall Business Performance

| Metric | Value |
|---|---:|
| Total Revenue | ₹655.23M |
| Total Orders | 10,000 |
| Average Rating | 4.0 |
| Total Profit | ₹71.58M |

### Business Interpretation

The mobile store shows strong overall performance with high revenue and a healthy order volume. However, deeper analysis shows that the mid-range phone segment plays a major role in driving customer interest and conversion opportunities.

---

## 📱 Mid-Range Phone Segment Performance

| Metric | Value |
|---|---:|
| Revenue | ₹154.37M |
| Total Orders | 4,073 |
| Average Rating | 4.0 |
| Profit | ₹21.54M |

### Segment Insight

Mid-range phones are a high-potential category because they attract customers who want a balance between **price, features, gaming experience, and everyday performance**.

This segment is especially important because it contributes a strong share of total orders and generates meaningful profit for the business.

---

## 🎮 Top Purchase Reasons for Mid-Range Phones

| Purchase Reason | Orders | Revenue | Profit | Order Share |
|---|---:|---:|---:|---:|
| Gaming | 1,868 | ₹93.99M | ₹12.48M | 45.86% |
| Features | 1,782 | ₹53.06M | ₹7.96M | 43.75% |
| Performance | 423 | ₹7.33M | ₹1.10M | 10.39% |

### Key Insight

Customers are not buying mid-range phones only because of price. The biggest purchase drivers are:

- Gaming experience
- Feature-rich usage
- Daily entertainment
- Value-for-money experience

This means marketing should focus less on generic performance claims and more on emotional, benefit-driven messaging such as:

> **“Best Gaming Phones Under ₹30K”**  
> **“Feature-Packed Phones for Everyday Entertainment”**  
> **“Powerful Experience Without Premium Pricing”**

---

## 💳 Payment Method Analysis

| Payment Method | Order Share |
|---|---:|
| Debit Card | 36.53% |
| UPI | 27.42% |
| Cash | 18.17% |
| Bank Transfer | 17.87% |

### Key Insight

Digital payments dominate the order share, especially debit cards and UPI. This indicates that customers are digitally comfortable and likely to respond well to instant payment-based offers.

### Business Opportunity

The store can improve conversions by offering:

- UPI cashback
- Debit card instant discounts
- No-cost EMI
- Limited-time payment offers
- Bank partner promotions

---

## 👥 Income Level vs Purchase Reason

| Income Level | Gaming | Features | Performance |
|---|---:|---:|---:|
| Low Income | 16.06% | 14.98% | 3.73% |
| Medium Income | 14.90% | 14.83% | 3.44% |
| High Income | 14.90% | 13.95% | 3.22% |

### Key Insight

Across all income levels, **Gaming** and **Features** remain the strongest buying motivations.

This shows that value-for-money is important, but customers are not only looking for the cheapest option. They want phones that feel powerful, useful, entertaining, and feature-packed.

### Business Meaning

The same campaign theme can work across multiple customer segments, but the message should be slightly personalized.

Examples:

| Customer Segment | Recommended Message |
|---|---|
| Low Income | Best Features at the Best Price |
| Medium Income | Gaming + Camera + Battery in One Phone |
| High Income | Premium Experience Without Premium Cost |

---

## 🏆 Top 10 Best-Selling Mid-Range Phones

<p align="center">
  <img src="assets/Best-Selling-Phone.png" width="100%" alt="Top 10 Best Selling Mid Range Phones" />
</p>

> Note: Store this image inside an `assets` folder in your GitHub repository and use the relative image path shown above.

---

## 💡 Key Business Insights

### 1. Gaming is the strongest purchase driver

Gaming contributes the highest order share and revenue among mid-range phone buyers. This means gaming-focused campaigns can directly influence conversion.

### 2. Features matter almost as much as gaming

Customers also care strongly about features such as camera, battery, display, storage, and everyday usability.

### 3. Performance alone is not the main selling point

Only a smaller percentage of customers selected performance as the main purchase reason. This suggests that technical performance should be translated into user benefits instead of being shown as raw specifications.

### 4. Digital payments create conversion opportunities

Debit cards and UPI together represent the majority of customer payment behavior. Payment-based offers can be a strong conversion lever.

### 5. Income level does not drastically change buying motivation

Gaming and features remain important across low, medium, and high-income customers. This means campaign messaging can be broad but still personalized by segment.

---

## 📢 Recommended Marketing Action Plan

### 1. Launch gaming-focused campaigns

Create banners and ad creatives such as:

- **Best Gaming Phones Under ₹30K**
- **Smooth Gaming. Powerful Battery. Great Price.**
- **Level Up Your Game Without Breaking Your Budget**

### 2. Promote feature-rich value messaging

Instead of only promoting discounts, highlight the complete user experience:

- Camera quality
- Battery life
- Storage
- Display
- Gaming performance
- Social media usage

Example campaign:

> **“Feature-Packed Phones for Work, Gaming, and Entertainment.”**

### 3. Add payment-based offers

Since digital payments are widely used, the business should run offers such as:

- 5% cashback on UPI
- Debit card instant discount
- No-cost EMI
- Bank partner offers
- Weekend payment deals

### 4. Personalize campaigns by customer segment

Use income level, rating category, phone model, and purchase reason to personalize campaigns.

Example:

| Segment | Campaign Idea |
|---|---|
| Gaming Buyers | Gaming phone bundles |
| Feature Buyers | Camera + battery campaigns |
| UPI Users | UPI cashback offers |
| High-Rating Models | “Top Rated by Customers” banners |

---

## 🧠 Final Business Recommendation

The analysis clearly shows that mid-range phone customers are **value-focused, digitally active, and experience-driven**.

To increase conversions, the business should focus on:

- Gaming-led campaigns
- Feature-focused product positioning
- UPI and debit card offers
- Customer segment-based personalization
- Highlighting top-rated and best-selling models

The strongest campaign message should not be only:

> “Affordable Phones”

Instead, it should be:

> **“Powerful, Feature-Packed Gaming Phones at the Right Price.”**

---

## ✅ Final Conclusion

This Power BI dashboard helped convert raw mobile sales data into clear business insights.

The analysis shows that mid-range smartphone buyers are mainly influenced by **gaming, features, digital payment convenience, and value-for-money positioning**.

By using these insights, the Mobile E-Store can create stronger campaigns, improve product positioning, and increase conversions in the mid-range phone segment.

---

## 🙋‍♂️ Author

**Masoom Naushad**  
Data Analyst | Business Intelligence | Power BI | SQL | Excel  

---
