import pandas as pd

# Load dataset
df = pd.read_csv("Customer Purchase Data.csv")

# -------------------------------
# 1. Basic Data Inspection
# -------------------------------
print("First 5 Rows:")
print(df.head())

print("\nDataset Info:")
print(df.info())

print("\nMissing Values:")
print(df.isnull().sum())

print("\nDuplicate Rows:")
print(df.duplicated().sum())

# -------------------------------
# 2. Data Cleaning
# -------------------------------

# Drop unnecessary column (ID column)
if "Number" in df.columns:
    df = df.drop(columns=["Number"])

# -------------------------------
# 3. Feature Engineering
# -------------------------------

# Create Customer Value
df['Customer_Value'] = df['Purchase_Frequency'] * df['Last_Purchase_Amount']

# Create Age Group
def categorize_age(age):
    if age < 30:
        return "Young"
    elif age < 50:
        return "Adult"
    else:
        return "Senior"

df['Age_Group'] = df['Age'].apply(categorize_age)

# -------------------------------
# 4. Final Check
# -------------------------------

print("\nCleaned Dataset Preview:")
print(df.head())

print("\nStatistical Summary:")
print(df.describe())

# -------------------------------
# 5. Save Cleaned Dataset
# -------------------------------

df.to_csv("cleaned_data.csv", index=False)

print("\nCleaned data saved successfully!")
