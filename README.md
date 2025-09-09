# Codeflix Churn Analysis

This project analyzes **subscription churn rates** for Codeflix, a streaming video startup. The goal is to provide insights into overall churn and compare churn between two distinct user acquisition segments.

---

## 📊 Project Overview

Four months after launch, Codeflix management requested an analysis of subscription churn rates. The marketing team was especially interested in understanding churn differences between two customer segments, defined by acquisition channel.

The project uses the provided dataset to:
- Calculate monthly churn rates.
- Compare churn between user segments.
- Highlight insights that can guide marketing and retention strategies.

---

## 🗂 Dataset

The dataset consists of a SQL table named **`subscriptions`** with the following columns:

| Column              | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `id`                | Unique subscription identifier.                                             |
| `subscription_start`| Start date of the subscription.                                              |
| `subscription_end`  | End date of the subscription (if applicable).                               |
| `segment`           | Acquisition segment to which the subscriber belongs.                        |

**Business Rule:**  
- Minimum subscription length is **31 days**, meaning a subscription cannot start and end within the same calendar month.

---

## 🧮 Key Definitions

- **Churned User**: A user whose `subscription_end` date falls within the observed time period.  
- **Active User**: A user whose subscription is ongoing at a given point in time.  
- **Churn Rate Formula**:  
  \[
  \text{Churn Rate} = \frac{\text{Number of Churned Users in Period}}{\text{Number of Active Users at Start of Period}}
  \]

---

## 🛠 Tools & Technologies

- **SQL**: Data extraction and churn calculation.  
- **SQL Workbench**: Query execution, analysis, and result exploration.  

---

## 🚀 How to Run the Project

1. **Set up the database**  
   - Import the `subscriptions` table into your SQL environment.

2. **Run SQL queries**  
   - Queries provided in this project calculate churn metrics and segment comparisons.


---

## 📈 Expected Outcomes

- Overall churn rate for Codeflix users.  
- Churn rate comparison between Segment A and Segment B.  
- Actionable insights for marketing and retention strategies.

---

## 🔮 Next Steps

- Extend analysis to include lifetime value (LTV).  
- Explore retention trends beyond the first four months.  
- Build predictive models for early churn detection.

---

## 📝 License

This project is for educational and analytical purposes. No proprietary Codeflix data is shared.
