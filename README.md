# 💳 UPI Fraud Analytics Dashboard

## 📊 Project Overview

The **UPI Fraud Analytics Dashboard** is an interactive **Power BI dashboard** designed to analyze UPI transaction data and identify fraud patterns.

The dashboard provides insights into transaction volume, fraud transactions, transaction amounts, fraud rates, and different factors associated with fraudulent activities.

It helps users understand **when, where, and how UPI fraud occurs** through interactive visualizations and filters.

---

## 🎯 Objectives

* Analyze UPI transaction and fraud data.
* Identify patterns and trends in fraudulent transactions.
* Calculate important fraud-related KPIs.
* Compare fraud across different categories.
* Identify high-risk transaction patterns.
* Provide an interactive dashboard for better decision-making.

---

## 🛠️ Tools & Technologies

* **Microsoft Power BI** – Dashboard and data visualization
* **Power Query** – Data cleaning and transformation
* **DAX** – Calculated measures and KPIs
* **CSV / Excel** – Dataset and data source

---

## 📌 Key KPIs

The dashboard provides important metrics such as:

* 💰 Total Transaction Amount
* 🔄 Total Transactions
* 🚨 Total Fraud Transactions
* 📈 Fraud Rate
* 💳 Average Transaction Amount
* 📊 Fraud Transaction Percentage

---

## 📊 Dashboard Features

### 1. Transaction Analysis

* Total number of UPI transactions
* Transaction amount analysis
* Average transaction value
* Transaction trends

### 2. Fraud Analysis

* Fraud vs. non-fraud transactions
* Fraud rate analysis
* Fraud transaction trends
* Fraud distribution across categories

### 3. Category Analysis

The dashboard allows fraud analysis based on available dataset attributes such as:

* Transaction Type
* Payment Method
* Location
* Device
* Customer Category
* Time/Date
* Transaction Amount

### 4. Interactive Filters

Users can interact with the dashboard using slicers and filters to analyze specific segments of the data.

Examples:

* Date
* Location
* Transaction Type
* Payment Method
* Fraud Status
* Customer Category

---

## 🔄 Data Preparation

The dataset was processed using **Power Query** before visualization.

The preprocessing steps included:

1. Loading the dataset into Power BI.
2. Checking and handling missing values.
3. Removing duplicate records where required.
4. Correcting data types.
5. Cleaning and standardizing categorical values.
6. Creating calculated columns where required.
7. Creating DAX measures for KPIs.
8. Building relationships between relevant tables.

---

## 📐 DAX Measures

Example measures used in the dashboard include:

```DAX
Total Transactions = COUNTROWS(Transactions)
```

```DAX
Fraud Transactions =
CALCULATE(
    COUNTROWS(Transactions),
    Transactions[Is_Fraud] = 1
)
```

```DAX
Fraud Rate =
DIVIDE(
    [Fraud Transactions],
    [Total Transactions],
    0
)
```

---

## 📈 Dashboard Insights

The dashboard can be used to identify:

* Fraud trends over time.
* Categories with higher fraud rates.
* Locations with increased fraudulent activity.
* Transaction types associated with higher fraud.
* Differences between fraudulent and legitimate transactions.
* High-value fraudulent transactions.
* Patterns that may indicate potential risk.

---

## 📂 Project Structure

```text
UPI_Fraud_Analytics_Dashboard/
│
├── UPI_Fraud_Analytics_Dashboard.pbix
├── README.md
│
├── dataset/
│   └── upi_fraud_data.csv
│
├── screenshots/
│   └── dashboard.png
│
└── documentation/
    └── Project_Report.pdf
```

---

## 🖼️ Dashboard Preview

Add your Power BI dashboard screenshot here:

```markdown
![UPI Fraud Analytics Dashboard](screenshots/dashboard.png)
```

---

## 🚀 How to Use

1. Clone this repository:

```bash
git clone https://github.com/UjjawalPrasad05/UPI_Fraud_Analytics_Dashboard.git
```

2. Open the project folder.
3. Open `UPI_Fraud_Analytics_Dashboard.pbix` using **Microsoft Power BI Desktop**.
4. If required, update the dataset path.
5. Refresh the data.
6. Use the available slicers and visualizations to explore the dashboard.

---

## 💡 Benefits

* Provides a centralized view of UPI fraud data.
* Makes fraud patterns easier to understand.
* Supports interactive data exploration.
* Helps identify high-risk transaction categories.
* Converts raw transaction data into meaningful insights.

---

## ⚠️ Limitations

* Dashboard accuracy depends on the quality of the dataset.
* Historical data may not represent current fraud patterns.
* The dashboard identifies patterns but does not guarantee that a transaction is fraudulent.
* Results are limited to the attributes available in the dataset.

---

## 🔮 Future Enhancements

Future improvements could include:

* 🤖 Machine Learning-based fraud prediction.
* Real-time transaction monitoring.
* Automated fraud alerts.
* Advanced anomaly detection.
* Risk scoring for individual transactions.
* Integration with live UPI transaction data.
* Deployment through Power BI Service.

---

## 👨‍💻 Author

**Ujjawal Prasad**

GitHub: [UjjawalPrasad05](https://github.com/UjjawalPrasad05)

---

## ⭐ Project

If you find this project useful, consider giving the repository a ⭐ on GitHub.
