🛒 E-Commerce Customer Segmentation & Churn Risk Analytics

An end-to-end data analytics project combining Python (Pandas, Scikit-learn) for behavioral customer segmentation (RFM + K-Means) and predictive churn modeling with an executive Power BI Dashboard delivering actionable retention strategies.

📌 Executive Summary & Business Objective

Customer acquisition costs continue to climb across retail, making retaining high-value accounts critical for long-term margins. This project analyzes transactional records from an e-commerce platform to:

Quantify Customer Behavior: Engineer Recency, Frequency, and Monetary (RFM) metrics alongside Average Order Value (AOV).

Cluster Customer Personas: Segment customers into distinct operational cohorts using unsupervised K-Means clustering.

Model Churn Risk: Identify early behavioral attrition signals using a Random Forest classification model (benchmarked at 90+ days of inactivity).

Drive Actionable Retention: Surface a targeted Power BI Watchlist for retention marketing teams to intervene before full churn occurs.

📊 Dashboard Previews

Page 1: Executive KPI & Segmentation Overview

Page 2: Churn Prevention & Retention Watchlist

🛠️ Tech Stack & Analytical Methods

Languages & Libraries: Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)

Business Intelligence: Microsoft Power BI Desktop (Star Schema Modeling, Custom DAX)

Feature Engineering: RFM Transformation, Log-scaling (np.log1p), StandardScaler

Machine Learning Algorithms:

Clustering: K-Means with Elbow Method (Inertia) & Silhouette Score optimization ($k = 4$)

Classification: Random Forest Classifier (Stratified Train/Test Split)

Key Metrics Tracked: Silhouette Score, Recall, ROC-AUC, Churn Rate %, Customer Lifetime Value (CLV), At-Risk Revenue

🔍 Key Insights & Business Recommendations

Revenue Concentration (The Pareto Dynamic):

The Champions segment accounts for less than 20% of the active customer base, yet generates over 50% of cumulative revenue.

Recommendation: Prioritize exclusive VIP perks, early product drops, and loyalty tiers to protect this core revenue engine.

Immediate At-Risk Exposure:

Over $1.4M in historical revenue is held by customers categorized as At-Risk (Recency > 90 days and high prior spend).

Recommendation: Deploy automated retention win-back campaigns offering targeted 15% discount incentives within a 14-day window.

Predictive Churn Detection:

The Random Forest model achieved 83% recall in identifying churn risk, demonstrating that order cadence drops and declining AOV serve as early indicators prior to complete inactivity.

📁 Repository Directory Structure

ecommerce-customer-segmentation-churn/
│
├── data/
│   └── customer_rfm_segments.csv       # Processed customer metrics & segment assignments
│
├── notebooks/
│   └── customer_segmentation.ipynb     # Data cleaning, RFM pipeline, and ML modeling
│
├── dashboard/
│   ├── customer_analytics.pbix         # Interactive Power BI report file
│   └── screenshots/
│       ├── executive_overview.png      # High-res screenshot of Dashboard Page 1
│       └── churn_watchlist.png         # High-res screenshot of Dashboard Page 2
│
├── requirements.txt                    # Project dependencies
└── README.md                           # Documentation & portfolio report


🚀 How to Run This Project Locally

1. Clone the Repository

git clone https://github.com/ZohraFathima0603/ecommerce-customer-segmentation-churn.git
cd ecommerce-customer-segmentation-churn


2. Set Up the Python Environment

pip install -r requirements.txt


3. Run the Jupyter Notebook

jupyter notebook notebooks/customer_segmentation.ipynb


4. Open the Power BI Dashboard

Open dashboard/customer_analytics.pbix with Power BI Desktop to view or modify the interactive visualizations and DAX measures.
