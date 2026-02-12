# Task15_RFM

⚙️ Project Workflow
1️⃣ Data Cleaning

Removed null CustomerID

Removed canceled invoices (InvoiceNo starting with 'C')

Converted InvoiceDate to datetime

Created Revenue = Quantity × UnitPrice

2️⃣ RFM Metric Calculation

Recency
Days since last purchase.


Recency=Snapshot Date−Last Invoice Date

Frequency
Number of unique invoices per customer.

Monetary
Total revenue per customer.

3️⃣ RFM Scoring

Used quantile binning (qcut).

Scores range from 1–4.

Combined into a 3-digit RFM score.

Example:

444 → Best customers

111 → Lowest engagement

4️⃣ Customer Segmentation Logic
Segment	Description
Champions	Recently active & frequent buyers
Loyal Customers	High frequency buyers
Potential Loyalist	Recently active but moderate frequency
At Risk	Not recent buyers
Lost	Long inactive customers
5️⃣ Visualization

Bar chart showing segment distribution

Helps understand customer base composition

📈 Business Actions Per Segment
🏆 Champions

VIP rewards

Early product access

Referral programs

🤝 Loyal Customers

Cross-sell recommendations

Loyalty points

Membership upgrades

🌱 Potential Loyalist

Targeted email campaigns

Limited-time offers

Engagement content

⚠️ At Risk

Win-back discounts

Feedback surveys

Personalized re-engagement

❌ Lost

Reactivation campaigns

Strong promotional offers

Churn analysis

📊 Why RFM?

RFM is used in:

E-commerce

Retail

Banking

Subscription businesses

CRM analytics

It enables behavioral segmentation instead of demographic-based segmentation.

✅ Validation of Segmentation

Segmentation usefulness can be validated by:

Revenue contribution by segment

Repeat purchase rate

Campaign conversion rate

Churn rate comparison

A/B testing results

🚀 Tools Used

Python

Pandas

NumPy

Matplotlib

Jupyter Notebook

🎯 Key Outcome

This project demonstrates:

Data cleaning and preprocessing

Customer behavioral analysis

Quantile-based segmentation

Business-driven insights

Marketing strategy alignment
