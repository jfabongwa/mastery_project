#  Customer Segmentation with Machine Learning

This project focuses on customer segmentation using a combination of **KMeans clustering**, **DBSCAN**, and **PCA**. The goal is to understand customer behavior and group similar customers together to inform business strategies like targeted marketing and customer retention.

---

## Project Overview

- **Objective**: Segment customers based on their demographic and booking behavior to identify distinct customer profiles.
- **Approach**: 
  - Rule-based segmentation using business logic on features like age, hotel/flight spend.
  - Unsupervised learning with KMeans and DBSCAN after dimensionality reduction using PCA.
  - Clusters are interpreted and labeled into customer personas for actionable insights.

---

## Tools & Libraries

- Python
- Jupyter Notebook
- pandas, numpy
- seaborn, matplotlib
- scikit-learn (KMeans, PCA, StandardScaler, LabelEncoder)
- statsmodels (for statistical insights if needed)

---

## Data Preparation

- Cleaned missing values and inconsistent entries
- Engineered features like:
  - `total_hotel_price`, `total_flight_price`
  - `avg_num_rooms`, `avg_new_nights`, etc.
- Encoded categorical features
- Normalized numerical features

---

## Methodology

1. **Dimensionality Reduction**
   - Used PCA to reduce feature space for clustering

2. **Clustering**
   - **KMeans**: Used the Elbow method and silhouette score to find optimal K
   - **DBSCAN**: Tuned `eps` and `min_samples` using silhouette and Davies-Bouldin Index

3. **Evaluation**
   - Silhouette Score
   - Davies-Bouldin Index
   - Cluster heatmaps for interpretation

4. **Labeling Clusters**
   - Clusters named based on summarized behavior:
     - `Balanced Explorers`
     - `High-End Vacationers`
     - `Business Jetsetters`
     - `Window Shoppers`

---

## Key Insights

- Identified **distinct segments** based on spending, travel frequency, and room preferences.

---

## 📁 Project Structure
├── data/
│ └── cleaned_customer_data.csv
├── notebooks/
│ └── customer_segmentation.ipynb
├── images/
│ └── cluster_heatmap.png
├── README.md
└── requirements.txt

## 🚀 Future Improvements

- Use **Time Series Forecasting** for customer lifetime value
- Apply **t-SNE** or **UMAP** for visual cluster separation
- Integrate with web dashboard for stakeholder presentation

---

## Contact

Feel free to reach out for questions or collaborations!

📧 jfabongwa@yahoo.com
🔗 [LinkedIn](https://www.linkedin.com/in/julius-abongwa-82235756/)
