# 📊 Olist Revenue & Order Analysis Report

This project analyzes Brazilian e-commerce data from Olist to derive meaningful insights into orders, revenue, freight cost, customer behavior, and payment methods. It follows a modern data stack approach using Google Cloud Storage, BigQuery, and Looker Studio.

## 📸 Snapshots

Here’s a preview of the interactive **Olist Revenue & Order Analysis Report** built using Looker Studio:

![Image](https://github.com/user-attachments/assets/9dc13b9f-d4f1-49c9-855c-4e23f8a81924)

![Image](https://github.com/user-attachments/assets/65dc8a05-9fe9-46b4-b6a6-325b907a19a1)

---

## 📁 Dataset Description

The dataset is sourced from the [Olist E-commerce Public Dataset Available in Data.world](https://data.world/adas086/olistcustomersdataset). It contains information on orders, customers, sellers, products, payments, reviews, and more.

### Tables Used:
1. `olist_orders_dataset.csv`
2. `olist_order_items_dataset.csv`
3. `olist_order_payments_dataset.csv`
4. `olist_order_reviews_dataset.csv`
5. `olist_customers_dataset.csv`
6. `olist_products_dataset.csv`
7. `olist_sellers_dataset.csv`

---

## ☁️ Project Workflow

### 🔹 Step 1: Data Storage in Google Cloud
- All 7 CSV files were uploaded and stored in **Google Cloud Storage (GCS)**.

### 🔹 Step 2: Creating External Tables in BigQuery
- Connected GCS to **BigQuery**.
- Created **external tables** for each CSV file (no ingestion needed).

### 🔹 Step 3: Data Transformation
- Cleaned and joined all 7 tables in BigQuery.
- Created a final **view table** containing all relevant columns:
  - Revenue
  - Freight value
  - Quantity sold
  - Order date
  - Profit (Revenue - Freight)
  - Payment type
  - Customer location
  - Product category
  - And more...

### 🔹 Step 4: Connecting to Looker Studio
- Connected the final view table from BigQuery to **Looker Studio** (formerly Data Studio).
- Built an interactive and filterable **Revenue & Order Analysis Report**.

---

## 📈 Key Features of the Report

- **KPI Cards**: Total Orders, Revenue, Freight, AOV (Average Order Value), Products Sold, and Quantity.
- **Time-Series Analysis**: Monthly breakdown of revenue, orders, profit, and quantity sold.
- **Category & State Rankings**: Top 5 product categories and states by revenue.
- **Payment Type Distribution**: Pie chart of profit % by payment methods.
- **Customer Segmentation**: Top customers by total revenue.
- **Weekday vs Weekend Revenue Split**.
- **Interactive Filters**: Seller state, city, order status, and payment type.
- **Date Range Picker**.

---

## 🛠 Tools & Technologies Used

| Tool            | Purpose                          |
|-----------------|----------------------------------|
| Google Cloud Storage | Cloud-based CSV storage        |
| BigQuery        | SQL-based data transformation     |
| Looker Studio   | Data visualization & reporting    |
| SQL             | Data joins, cleaning, and logic   |

---

## 📌 Outcome

A complete end-to-end **business report** that allows stakeholders to:
- Monitor monthly performance.
- Understand revenue drivers.
- Analyze customer and product trends.
- Make data-driven decisions using a dynamic report.

---

## 📎 Folder Structure


---

## 🔗 Live Report Link

👉 [View the Report in Looker Studio](https://lookerstudio.google.com/s/uMhGSWnsufw)  


---

## 📬 Contact

**Created by:** Arshad  
Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/mohd-arshad-726b38286/) or check out my [YouTube SQL Projects](https://www.youtube.com/@Arshad_Data_Analyst).

---



