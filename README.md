# 🛍️ Customer Segmentation using KMeans Clustering and PCA

This project performs customer segmentation on a mall dataset using **KMeans Clustering** and **Principal Component Analysis (PCA)**. It aims to group customers based on their demographics and spending patterns to help businesses target marketing strategies more effectively.

---

## 📂 Dataset Features

The dataset contains the following features:

- `CustomerID`: Unique ID for each customer (removed before clustering)
- `Gender`: Male or Female
- `Age`: Age of the customer
- `Annual Income (k$)`: Annual income in thousands of dollars
- `Spending Score (1–100)`: Score assigned by the mall based on customer behavior and spending nature

---

## 📌 Objectives

- Preprocess the dataset and handle categorical data
- Standardize features
- Apply **PCA** to reduce dimensions for visualization
- Use **KMeans Clustering** to segment customers
- Assign intuitive labels to each cluster
- Visualize the clusters and profile each group

---

## 🧪 Technologies Used

- Python 🐍
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (KMeans, PCA, preprocessing)

---

## 🧮 Project Workflow

1. **Data Cleaning & Preprocessing**
   - Removed `CustomerID`
   - Encoded `Gender`
   - Standardized numerical features

2. **PCA for Dimensionality Reduction**
   - Reduced to 2D for better cluster visualization

3. **KMeans Clustering**
   - Elbow and Silhouette methods to determine optimal clusters (chose 4)
   - Clustered customers based on PCA-transformed data

4. **Cluster Labeling**
   - Clusters labeled for interpretability:
     - `Wealthy Spenders`
     - `Struggling Youth`
     - `Spontaneous Shoppers`
     - `Careful Rich`

5. **Visualization**
   - 2D scatter plot of PCA components colored by clusters
   - Cluster profiling based on mean values

---

## 📊 Cluster Labels & Interpretation

| Cluster | Label                 | Characteristics                                     |
|---------|-----------------------|------------------------------------------------------|
| 0       | Careful Rich          | High income, low spending                           |
| 1       | Struggling Youth      | Low income, low spending                            |
| 2       | Spontaneous Shoppers  | Young, low income, but high spending                |
| 3       | Wealthy Spenders      | High income, high spending                          |

---

## 📁 Files in this Repository

- `customer_segmentation.ipynb`: Jupyter notebook with all code
- `dataset.csv`: Input dataset
- `README.md`: Project documentation
- `segmented_customers.csv`: Output with segment labels (optional)

---

## 🧠 Conclusion

KMeans clustering combined with PCA proves to be a powerful method for segmenting customers. The insights gained can help businesses design targeted campaigns and better allocate resources.

---

## 📬 Contact

Feel free to reach out if you have any questions or suggestions!
