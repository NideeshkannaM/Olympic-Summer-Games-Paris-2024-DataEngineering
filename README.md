## ⚙️ Tools & Technologies Used

- **Azure Data Factory** – Ingest raw Olympic data from GitHub into Azure Data Lake
- **Azure Data Lake Storage** – Central storage for raw and transformed data
- **Azure Databricks (PySpark)** – Cleanse, transform, and analyze the datasets
- **Delta Lake** – For ACID-compliant storage format
- **GitHub** – Version control for notebooks, pipeline definitions, and scripts

---

## 🛠️ Data Pipeline Workflow

### 🔹 Step 1: Data Ingestion
- **Source**: Kaggle Paris Olympic Dataset
- **Tool**: Azure Data Factory
- **Destination**: Azure Data Lake Storage Gen2

### 🔹 Step 2: Data Transformation & Processing
- **Tool**: Azure Databricks (PySpark)
- **Process**:
  - Clean missing or malformed records
  - Normalize country codes and event types
  - Join and enrich datasets (athletes, coaches, events, medals)
  - Persist cleaned data in Delta format

### 🔹 Step 3: Analysis & Insights
- Interactive visuals created for:
  - **Country-Wise Gender-Wise Medal Count**
  - **Event Type with Most Participation**
  - **Medal Efficiency Country Wise**

---

## 📊 Sample Visual Outputs
1) Country-Wise Gender-Wise Medal Count Visualization
<img width="1382" height="582" alt="image" src="https://github.com/user-attachments/assets/a81dfe71-50f2-4bde-945d-04967637fe5e" />

2) Event Type with Most Participation
<img width="1339" height="522" alt="image" src="https://github.com/user-attachments/assets/e3d52121-af8d-4122-b6bd-b597ed2bd421" />

3) Medal Efficiency Country Wise
<img width="1428" height="522" alt="image" src="https://github.com/user-attachments/assets/36a34e42-d24d-46df-bee7-d8f07c178de3" />

---

## 🚀 Future Enhancements

- Add more KPI's based on the available data
- Connect to Power BI or Synapse Analytics for business-level dashboards
- Add real-time ingestion using Event Hubs (optional expansion)
