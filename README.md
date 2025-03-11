# Customer Segmentation using KMeans Clustering

## 📌 Project Overview
This project applies **KMeans clustering** to segment customers based on their purchasing behavior using an online retail dataset. The goal is to identify actionable customer groups for better marketing and retention strategies.

## 📂 Dataset
The dataset contains transactional data from an online retail store, including:
- **InvoiceNo**: Unique transaction ID
- **StockCode**: Product code
- **Description**: Product description
- **Quantity**: Number of items purchased
- **InvoiceDate**: Date of transaction
- **UnitPrice**: Price per item
- **CustomerID**: Unique identifier for customers
- **Country**: Customer's location

The dataset is available at: [Online Retail II Dataset](https://archive.ics.uci.edu/dataset/502/online+retail+ii)

## 🚀 Methodology
### 1️⃣ Data Preprocessing
- Removed missing values and invalid transactions
- Filtered out refunds (negative quantities)
- Computed **Monetary Value**, **Frequency**, and **Recency** features

### 2️⃣ Feature Engineering
- **Recency**: Days since last purchase
- **Frequency**: Number of transactions
- **Monetary Value**: Total spending
- Applied **StandardScaler** for normalization

### 3️⃣ Clustering using KMeans
- Determined the optimal number of clusters using **Elbow Method** (Inertia) & **Silhouette Score**
- Applied **KMeans clustering** to segment customers

### 4️⃣ Cluster Analysis & Interpretation
- Used **3D scatter plots** for visualization
- Identified three customer segments:
  - **Retain**: High-value, loyal customers
  - **Re-Engage**: Low-value, infrequent buyers
  - **Nurture**: Recent buyers with lower engagement

## 📊 Visualizations
- **Elbow Method Plot** to determine optimal clusters
- **3D Scatter Plot** for customer segmentation
- **Violin Plots** to compare cluster distributions

## 🛠️ Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn (KMeans, StandardScaler)
- Matplotlib, Seaborn

## 📈 Results & Insights
- **High-value customers** contribute the most to revenue → Priority for retention.
- **Infrequent buyers** need marketing efforts to increase engagement.
- **Recent buyers** have potential to be nurtured into loyal customers.

## 📌 How to Run the Project
### Prerequisites
Ensure you have Python installed and the required libraries:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

### Running the Script
```bash
python customer_segmentation.py
```

## 🔗 Future Improvements
- Explore **Hierarchical Clustering** and **DBSCAN** for comparison
- Implement **Customer Lifetime Value (CLV)** predictions
- Apply **Deep Learning** for more advanced segmentation

## 📜 License
This project is open-source under the [MIT License](LICENSE). Feel free to contribute!

## 🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

## 📬 Contact
For any queries, reach out via [GitHub Issues](https://github.com/UtkarshMidha/Customer-Segmentation-using-KMeans-Clustering/issues).
