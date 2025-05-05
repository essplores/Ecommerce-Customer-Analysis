# Ecommerce-Customer-Analysis
This project analyzes eCommerce customer data to extract actionable insights around sales trends, product performance, customer segmentation, and retention strategies using Python.

## 📊 Project Objectives
- Identify top-performing product categories and sales trends
- Understand seasonal revenue patterns
- Segment customers by recency and demographic behavior
- Analyze basket size and pricing sensitivity
- Investigate return rates and churn risk

## 🧰 Tools & Technologies
- Python (Pandas, NumPy)
- Data Visualization: Matplotlib, Seaborn
- Jupyter Notebook
- Data size: ~250k rows (CSV)

### 🛍️ Sales & Category Analysis
| Product Category | Total Revenue | Total Quantity | Average Price | Number of Orders | Revenue Share | Cumulative Share | Top 80% |
|------------------|---------------|----------------|----------------|------------------|----------------|-------------------|----------|
| Home             | 171,138,916   | 188,077        | 255.64         | 62,542           | 25.12%         | 25.12%            | ✅       |
| Clothing         | 170,716,122   | 188,688        | 254.32         | 62,581           | 25.06%         | 50.17%            | ✅       |
| Electronics      | 170,146,025   | 187,861        | 254.28         | 62,630           | 24.97%         | 75.15%            | ✅       |
| Books            | 169,345,236   | 186,608        | 254.72         | 62,247           | 24.85%         | 100.00%           | ❌       |

- Top 3 product categories contribute **~75% of revenue** (Pareto principle)
- **Books** have a high return rate (>50%) despite strong sales

### 📅 Seasonality
![image](https://github.com/user-attachments/assets/e436bb38-4553-4437-a955-8a53833b892e)
![image](https://github.com/user-attachments/assets/b81baf86-0e2d-46c4-bd9d-0b201b4a3d9f)
- Clear revenue peaks in **May, July, and December** depending on category

### 👤 Customer Segmentation
![image](https://github.com/user-attachments/assets/50f5f1c4-b935-41a9-822a-81d667092a95)
- Majority of customers are **churned (71%)**, with only 11% active
- Older customers (55–64) have **higher AOV** and generate more revenue
- Basket size is consistent (~3 items), but older users spend more per item

| Age Group | Gender | Avg Basket Size | Avg Purchase Amount | Transaction Count |
|-----------|--------|------------------|----------------------|-------------------|
| 18–24     | Female | 3.01             | 2,602.23             | 16,993            |
| 18–24     | Male   | 3.02             | 2,608.13             | 17,197            |
| 25–34     | Female | 3.01             | 2,655.10             | 23,979            |
| 25–34     | Male   | 2.99             | 2,673.19             | 23,635            |
| 35–44     | Female | 3.00             | 2,704.81             | 23,256            |
| 35–44     | Male   | 3.00             | 2,697.13             | 23,569            |
| 45–54     | Female | 3.01             | 2,755.84             | 22,824            |
| 45–54     | Male   | 3.01             | 2,763.78             | 23,670            |
| 55–64     | Female | 3.01             | 2,815.09             | 23,003            |
| 55–64     | Male   | 3.00             | 2,819.46             | 23,503            |
| 65+       | Female | 3.02             | 2,843.17             | 11,969            |
| 65+       | Male   | 2.99             | 2,850.20             | 11,614            |

### 💳 Pricing Sensitivity
![image](https://github.com/user-attachments/assets/8f8b1dbd-432f-497c-a3a7-f096d80416f9)
| Payment Method | Avg Basket Size | Avg Purchase Amount | Transaction Count |
|----------------|------------------|----------------------|-------------------|
| Cash           | 3.00             | 2,715.56             | 83,012            |
| Credit Card    | 3.00             | 2,738.85             | 83,547            |
| PayPal         | 3.01             | 2,721.68             | 83,441            |

- Credit card users show slightly **higher AOV**, indicating premium preference
- Younger buyers are more **price-sensitive**, suggesting bundle/discount opportunities

## 🧪 Files in This Repository

- `ecommerce_customer_data_large.csv` – anonymized transactional dataset
- `notebook.ipynb` – full Python notebook with code and visualizations
- `plots/` – folder containing key visual outputs
- `report_summary.pdf` – optional summary report version (if included)

---

## 📌 Next Steps

- Develop **churn prediction model**
- Build **RFM segmentation**
- Create **interactive dashboard** (Power BI or Streamlit)
