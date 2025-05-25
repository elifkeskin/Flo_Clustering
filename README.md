
# Flo_Clustering: Spark Machine Learning Clustering for Customer Segmentation

## 📝 Business Problem

FLO aims to segment its customers to develop targeted marketing strategies. By analyzing customer behavior, the company seeks to define meaningful groups (clusters) and tailor its marketing efforts accordingly.

## 📂 Dataset Story

The dataset contains information about OmniChannel customers (both online and offline shoppers) who made their last purchases from FLO between 2020 and 2021. It includes historical shopping behavior and channel usage data.

## 🎯 Project Goal

The main objective is to segment FLO customers based on their shopping behaviors using Spark Machine Learning clustering algorithms. These segments will help inform and optimize marketing strategies.

## 🗃️ Data Fields

- **master_id:** Unique customer identifier.
- **order_channel:** Shopping platform used (Android, iOS, Desktop, Mobile).
- **last_order_channel:** Channel where the last purchase was made.
- **first_order_date:** Date of the customer's first purchase.
- **last_order_date:** Date of the customer's last purchase.
- **last_order_date_online:** Date of the customer's last online purchase.
- **last_order_date_offline:** Date of the customer's last offline purchase.
- **order_num_total_ever_online:** Total number of online purchases made by the customer.

## 🛠️ Technologies & Libraries

- **Apache Spark:** Distributed data processing and machine learning.
- **PySpark:** Python API for Spark.
- **pandas:** Data manipulation and analysis (for initial exploration).
- **matplotlib / seaborn:** Data visualization (optional).

## 🚦 Project Steps

1. **Data Loading & Exploration:**  
   - Import the dataset into Spark and perform initial exploratory data analysis.

2. **Data Preprocessing:**  
   - Handle missing values and outliers.
   - Convert date fields to appropriate formats.
   - Feature engineering (e.g., recency, frequency, monetary value calculations).

3. **Clustering:**  
   - Apply Spark ML clustering algorithms (e.g., KMeans) to segment customers based on behavioral features.

4. **Cluster Analysis:**  
   - Interpret and profile each customer segment.
   - Visualize cluster characteristics and provide actionable insights.

5. **Marketing Strategy Recommendations:**  
   - Suggest marketing actions for each identified customer segment.

## 🚀 Getting Started

1. **Clone the Repository**
    ```bash
    git clone https://github.com/elifkeskin/Flo-Clustering.git
    cd Flo-Clustering
    ```

2. **Install Dependencies**
    - Make sure you have Apache Spark and PySpark installed.
    - Install other required Python packages:
      ```bash
      pip install -r requirements.txt
      ```

3. **Run the Project**
    - Open the main script or Databricks notebook and follow the steps for data preprocessing, clustering, and analysis.

## 📊 Example Output

| Cluster | Number of Customers | Key Behaviors                | Suggested Strategy         |
|---------|---------------------|------------------------------|---------------------------|
| 0       | 1,200               | High online frequency        | Loyalty program           |
| 1       | 800                 | Recent offline shoppers      | In-store promotions       |
| ...     | ...                 | ...                          | ...                       |

## 🤝 Contributing

Contributions are welcome!  
1. Fork the repository  
2. Create a new branch (`git checkout -b feature-branch`)  
3. Commit your changes (`git commit -m 'Add new feature'`)  
4. Push to the branch (`git push origin feature-branch`)  
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License.

---

**For questions or suggestions, feel free to open an issue or contact the maintainer.**
