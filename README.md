# Customer Churn Analysis Pipeline

An end-to-end data analytics and churn prediction pipeline built for an OTT subscription platform. This project extracts relational data using SQLite, processes and cleans datasets in Python, and performs exploratory data analysis (EDA) to uncover key retention drivers and business insights.

---

## Project Overview

Customer churn is a critical challenge for subscription-based business models. The objective of this project is to build an automated analytics pipeline that tracks key performance indicators (KPIs), evaluates customer behavior, and identifies high-risk subscriber segments to support proactive retention strategies.

### Key Insights & Findings
* **Overall Metrics:** The dataset tracks an average churn rate of **31.9%** across a subscriber base of over 15,000 users.
* **Contract Impact:** Monthly-contract subscribers experience significantly higher churn compared to annual subscribers (**55.6% vs. 8.3%**).
* **Support Escalations:** Exploratory correlation analysis reveals a strong positive link between customer support escalations/tickets and churn risk.
* **Geographic Variations:** Regional analysis highlights distinct outliers, such as Karnataka showing higher churn concentrations compared to other regions.

---

## Tech Stack & Tools

* **Language:** Python 3.x
* **Database:** SQLite
* **Data Manipulation & Analysis:** `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`
* **Environment:** Jupyter Notebook / VS Code

---

##  Repository Structure

```text
customer-churn-analysis/
│
├── data/
│   └── churn_data.db          # SQLite database / schema files
│
├── notebooks/
│   └── churn_analysis.ipynb   # Main Jupyter Notebook containing EDA & queries
│
├── scripts/
│   └── data_loader.py         # Modular Python scripts for data extraction
│
├── visualisations/
│   ├── correlation_heatmap.png # Feature correlation matrix
│   ├── monthly_churn_trend.png # Churn trends over time
│   └── churn_by_state.png     # Geographic distribution of churn
│
├── .gitignore
├── requirements.txt           # Project dependencies
└── README.md                  # Project documentation

# Key Visualizations & EDA
1. Feature Correlation Heatmap
The correlation matrix analyzes the linear relationships between numeric features, plan types, contract types, and escalation metrics.

2. Monthly Churn Trend
Tracking the fluctuation of churned customers across active months to identify seasonal spikes or operational anomalies.

3. Churn Rate by State
Geographic breakdown illustrating regional variances in subscriber drop-offs.

# How to Run Locally
Clone the repository:
git clone [https://github.com/your-username/customer-churn-analysis.git](https://github.com/your-username/customer-churn-analysis.git)
cd customer-churn-analysis

# Install dependencies:
pip install -r requirements.txt

# Run the analysis:
Open and execute notebooks/churn_analysis.ipynb in Jupyter Notebook or VS Code.

# Strategic Recommendations
Contract Incentives: Deploy targeted discount incentives or onboarding promotions to transition high-risk monthly subscribers to annual plans.

Support Optimization: Streamline first-contact resolution pathways to address support ticket escalations before they result in subscriber cancellation.

Proactive Monitoring: Utilize churn risk scoring flags to trigger automated retention workflows when customer engagement drops.
