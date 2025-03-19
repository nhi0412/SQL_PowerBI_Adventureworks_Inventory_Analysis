# SQL_PowerBI_Adventureworks_Inventory_Analysis

## 1. Introduction and Motivation

In manufacturing, procurement ensures materials are purchased in sufficient quantities, on time, and at an optimized cost. An efficient system maintains supply flow, reduces costs, and enhances operations.

However, without data-driven insights, organizations risk stock shortages, delays, and high costs. To address this, leadership requires a clear, intuitive dashboard for better procurement decisions.

## **2. Introduction to Dataset**

Dataset: **adventureworks2019** (public Google BigQuery dataset)

[Dataset dictionary](https://drive.google.com/file/d/1oYm32cdutBwHhkds4l-HznDYPZ5_WCxu/view)

Key aspects from dataset such as:

- **Purchase orders** (order quantities, delivery timelines, vendors)
- **Inventory levels** (stock quantity, safety stock, reorder points)
- **Cost data** (standard price, last receipt cost, price variance)
- **Supplier performance** (on-time delivery rate, rejection rate)

## **3. Import Raw Data**

To access the AdventureWorks2019 eCommerce dataset in Google BigQuery's public datasets, follow these steps:

1. Sign in to your Google Cloud Platform (GCP) account and create a new project.
2. Open the BigQuery console and star the dataset for easy access.
3. In the console, enter the project name “adventureworks2019” and press Enter.
4. Navigate to the tables within the dataset.

## **4. Business Questions**

1. Are we purchasing enough stock to meet sales demands?
2. Are orders being delivered on time to avoid production delays?
3. Are procurement costs optimized across different vendors and products?
4. Which vendors have the highest rejection rates and cost variances?
5. How do procurement trends change over time, and what strategies can improve performance?

## 5. Design Thinking

### Empathize – Understanding Stakeholder' Needs

<img width="1191" alt="Image" src="https://github.com/user-attachments/assets/831d301c-b907-4d36-95fb-f15a95fdc7e2" />

<img width="793" alt="Image" src="https://github.com/user-attachments/assets/a701ff7a-d179-4dbc-93e6-d0ffaf6a724c" />

<img width="432" alt="Image" src="https://github.com/user-attachments/assets/1e7ea4ae-6a1f-4540-9bd4-ad7808b6ddb1" />


### Define – Defining the Point of View

<img width="645" alt="Image" src="https://github.com/user-attachments/assets/c206e33e-9e07-4306-9d57-9554f141d999" />

<img width="563" alt="Image" src="https://github.com/user-attachments/assets/72685c17-b24e-4659-af15-e43720ad8b3d" />

### **Ideate – Brainstorming Dashboard Components**

<img width="1160" alt="Image" src="https://github.com/user-attachments/assets/63100810-e216-4a05-a8e3-ab3a2fc04392" />

### Prototype and Review

Build a PowerBI dashboard and review each part.

## 6. Visualization

### Overview

<img width="851" alt="Image" src="https://github.com/user-attachments/assets/b8c04c06-3a74-4c46-92a3-482a421b9967" />

### Inventory Detail

<img width="850" alt="Image" src="https://github.com/user-attachments/assets/e6395d66-1d5b-4454-8613-070220babf6e" />

The inventory details dashboard provides detailed insights into specific products, helping track stock levels, reorder needs, and overall inventory performance.

- Users can search for product information using product name or product ID to quickly access relevant details.
- The order quantity by subcategory helps analyze demand patterns and identify high-performing product groups.
- A comparison between total stock, reorder point, and safety stock level ensures timely replenishment and prevents stockouts.
- The total order quantity over time visualization helps track product demand trends, allowing better forecasting and procurement planning.

## 6. Insights

- The majority of orders are shipped via Cargo Transport 5 (38%) and Overnight J Fast (27%), while Oversea-Deluxe has the least orders.
- The product under safety stock level table highlights stock shortages, helping the procurement team track and reorder necessary products.
- Rejection rate peaked in 2012 at 11.10%, significantly higher than in 2014 (2.09%), showing fluctuations in product quality over time.
- The scatter plot clearly identifies vendors with high rejection order quantity (SuperStores 6,373) and high price variances (Superior Bicycles 3.94), making it easier to assess supplier performance.

## **7. Recommendations**

### **Improve Shipping & Delivery Performance**

- Review the cost-effectiveness of different shipping modes and optimize logistics to reduce delivery delays and unnecessary costs.
- Use historical on-time delivery data to prioritize reliable shipping options.

### **Optimize Inventory Management**

- Set up automatic alerts when stock levels drop below the safety threshold to prevent stockouts and disruptions.
- Analyze total order quantity trends over time to predict demand and adjust inventory planning accordingly.

### **Strengthen Supplier & Cost Control Strategies**

- Monitor vendor performance regularly using rejection rates and price variances to negotiate better terms or find alternative suppliers.
- Apply stricter quality control measures for vendors with high rejection rates to minimize waste and defective goods.
- Consider bulk purchasing from reliable suppliers to secure better pricing and reduce overall procurement costs.
