# Task 1: Data Immersion & Wrangling

## 📌 Objective
The objective of this task is to understand, clean, and prepare a dataset for analysis. This includes identifying data quality issues, performing necessary cleaning steps, and transforming the dataset into an analysis-ready format.

---

## 📊 Dataset Description
The dataset contains customer-related information such as age, income, spending behavior, membership duration, and purchase details.

### Features:
- Age: Age of the customer
- Income: Annual income of the customer
- Spending_Score: Score based on spending behavior
- Membership_Years: Number of years the customer has been a member
- Purchase_Frequency: Frequency of purchases
- Last_Purchase_Amount: Amount spent in the last purchase

---

## 🔍 Data Quality Checks

The following checks were performed:

- Missing Values: No missing values were found in the dataset.
- Duplicate Records: No duplicate rows were identified.
- Data Types: All columns had appropriate data types and required no correction.

---

## 🛠 Data Cleaning Steps

- Removed the unnecessary column `Number` (identifier column).
- Verified dataset integrity (no missing or duplicate values).
- Standardized data formats where required.

---

## ⚙️ Feature Engineering

The following new features were created:

- **Customer_Value** = Purchase_Frequency × Last_Purchase_Amount  
  (Represents overall customer contribution)

- **Age_Group**:
  - Young: Age < 30
  - Adult: 30 ≤ Age < 50
  - Senior: Age ≥ 50

---

## 📈 Final Output

- A cleaned dataset (`cleaned_data.csv`) ready for analysis
- Python code used for cleaning and transformation
- Data dictionary explaining all variables

---

## 🧰 Tools & Technologies Used

- Python
- Pandas
- Google Colab

---

## ✅ Conclusion

The dataset was already well-structured with no missing or duplicate values. Key preprocessing steps included removing irrelevant columns and creating new features to enhance analytical capability. The final dataset is clean, structured, and ready for further analysis.
