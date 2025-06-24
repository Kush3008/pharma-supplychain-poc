# 💊 Pharma Supply Chain Data Pipeline (POC)

## 🎯 Goal
Build a modern data pipeline using `dbt`, `BigQuery`, and `Looker Studio` to clean, transform, validate, and visualize pharmaceutical delivery data.

## 🧰 Tools Used
- Python (pandas, faker)
- dbt (data modeling, transformation, testing)
- Google BigQuery (cloud data warehouse)
- Looker Studio (dashboard)
- GitHub (repo hosting)

## 📁 Project Structure
pharma_poc/
├── models/
├── data/
├── enrich_pii_dataset.py
├── packages.yml
├── README.md
## 🧪 Key Features
- Masked PII fields (Aadhaar, DOB, Phone, Email)
- Derived fields like `delivery_lag`, `value_per_kg`
- Summary aggregation by shipment mode & country
- Data tests with `dbt-utils`
- Fully styled interactive Looker dashboard

## 🚀 How to Reproduce
1. Clone repo
2. Upload `SCMS_with_PII.csv` to BigQuery
3. Configure `profiles.yml` and service account
4. Run:
```bash
dbt run
dbt test
dbt docs generate
