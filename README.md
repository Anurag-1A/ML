# Myntra Customer Segmentation (Unsupervised ML)

Myntra, a prominent Indian fashion e-commerce company, is celebrated for its extensive range of clothing, accessories, and lifestyle products. Beyond its fashion expertise, Myntra manages a specialized division Myntra Gifts Ltd. which focuses on unique, all-occasion giftware. Headquartered in the UK, this division serves international markets through its online retail platform

This aim of this project is to perform an exploratory data analysis to understand the dataset and uncover the underlying insights and the application of **Unsupervised Machine Learning** to segment Myntra customers based on purchasing behavior using **RFM analysis** and **KMeans clustering**. 

---

##  Problem Statement
In a competitive e-commerce space, it's crucial to understand and categorize customers based on their engagement. The goal is to:
- Segment customers using **Recency**, **Frequency**, and **Monetary** metrics.
- These customer segments will help the business better understand purchasing patterns, personalize marketing strategies, and improve customer retention through targeted engagement.

---

##  Dataset
The dataset contains transactions from December 1, 2009, to December 9, 2011.
- 'InvoiceNo'
- 'StockCode'
- 'Description'
- 'Quantity'
- 'InvoiceDate'
- 'UnitPrice'
- 'CustomerID'
- 'Country'.

> *Note: Synthetic/representative data used for analysis.*

---

## Approach

1. **Data Preprocessing**
   - Removed null/duplicate values
   - Applied **log transformation** and **standardization**
   - Calculating RFM metrics

2. **RFM Analysis**
   - Derived Recency, Frequency, and Monetary values per customer

3. **Clustering Techniques**
   - Used **KMeans** and **Hierarchical Clustering**
   - Evaluated using **Silhouette Score** and **Elbow Method**

4. **Cluster Profiling**
   - Labeled segments with business logic
   - Mapped clusters back to RFM dataframe for insight

---

# Identifying ideal number of clusters also depends upon the business requirement and cluster definition 

##  Key Insights

| Cluster | Segment                   | Behavior Description                             |
|---------|---------------------------|--------------------------------------------------|
| 0       | Loyal Mid Spenders        | Frequent, recent customers with moderate spend   |
| 1       | VIP/High value Customers  | Very frequent, recent, high-spending customers   |
| 2       | Frequent Buyers           | Often shop but spend modestly                    |
| 3       | Churned/At-Risk Customers | Long inactive, low frequency and low spend       |

---

##  Visualizations

-  Barchart
-  Heatmap 
-  Line chart (for hour/day sales trend)
-  Silhouette plots for cluster evaluation

---

##  Tools & Libraries

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn (KMeans, Silhouette Score, hierarchical clustering)
- Yellowbrick (Silhouette Visualizer)

---

## Business Impact
- RFM analysis and customer segmentation (via clustering) helps in identifying high-value customers. 
- Improved Product and Inventory Strategy:Product and customer behavior/ insights can help in inventory management by identifying which products are in higher demand helping businesses plan inventory management more efficiently and reduce overstock or stockouts.
- Operational Efficiency: Identifying periods of lower sales or dips in customer engagement allows companies to optimize their operational processes, ensuring smoother operations


---


