Data Cleaning – Marketing Campaign Dataset

Task Overview:

This task involves cleaning and preprocessing the Marketing Campaign dataset to make it ready for analysis. The dataset contained missing values, inconsistent formats, and required type conversions.

🔄 Steps Performed

Loaded dataset

File was tab-separated (TSV) → used sep="\t" for correct parsing.

Standardized column names

Converted all column names to lowercase

Replaced spaces with underscores (e.g., Year_Birth → year_birth).

Converted data types

dt_customer → converted to datetime

Numeric fields (income, recency, mnt_wines, etc.) → converted to proper numeric types.

Created derived column

Added new column age = 2025 - year_birth.

Cleaned categorical fields

Standardized text values in education and marital_status.

Handled missing values

Numeric columns → filled with median

Categorical columns → filled with mode (most frequent value).

Removed duplicates

Dropped duplicate rows (based on id).

Final dataset saved

Output file: marketing_campaign_cleaned.csv

Final shape: 2240 rows × 30 columns

📂 Repository Contents

marketing_campaign.csv → Original dataset

marketing_campaign_cleaned.csv → Cleaned dataset

clean_marketing_campaign.py → Python script for cleaning

README.md → Summary of steps

✅ Outcome

Dataset is now clean, structured, and ready for further analysis & modeling.

This process ensures better data quality and reliability for insights.
