# Smartcard Customer Insights

This repository contains a project that performs customer segmentation for a smart‑card dataset using agglomerative hierarchical clustering. The goal is to group customers into meaningful segments based on their transactional behaviour and demographic information, enabling data‑driven insights for marketing and product strategies.

## 📁 Project Structure

```
Smartcard-Customer-insights/
├── Smartcard Customer Insights/
│   ├── E_commerse_segmentation.ipynb   # Jupyter notebook with full analysis
│   └── smartcart_customers.csv         # Dataset used for clustering
└── README.md                          # This file
```

## 📝 Dataset

The `smartcart_customers.csv` file contains anonymized customer records with features such as:

- `CustomerID` – unique identifier
- `Age` – age of the customer
- `Annual_Income` – income bracket or yearly income
- `Spending_Score` – metric reflecting purchase behaviour
- ...and potentially other behavioural or demographic attributes

> **Note:** The notebook shows any feature preprocessing steps (scaling, encoding, etc.) before clustering.

## 🔍 Analysis Overview

1. **Data Loading & Exploration** – read in the CSV, inspect missing values, perform basic statistics and visualizations to understand feature distributions.
2. **Preprocessing** – standardization/normalization of numerical features and handling of any categorical variables.
3. **Clustering with Agglomerative Hierarchical Clustering**
   - A dendrogram is plotted to decide the number of clusters.
   - Model is fit to the data using ward linkage (or another linkage method as shown).
   - Cluster labels are assigned back to the dataset.
4. **Cluster Evaluation** – compute silhouette score or other metrics and visualize clusters with scatter plots.
5. **Insights & Interpretation** – describe characteristics of each segment (e.g., high-income high-spenders). Results are discussed in notebook cells.

## 🚀 How to Run

1. Make sure you have Python and Jupyter installed.
2. Navigate into the project directory:

   ```bash
   cd "Smartcard-Customer-insights/Smartcard Customer Insights"
   ```

3. Launch Jupyter Notebook and open `E_commerse_segmentation.ipynb`:

   ```bash
   jupyter notebook
   ```

4. Execute the cells sequentially to reproduce the analysis.

## 🛠 Dependencies

Typical packages used include:

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib` / `seaborn`
- `scipy` (for dendrogram)

Install via:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn scipy
```

## ✍️ Notes

- Feel free to extend the notebook with alternative clustering methods (KMeans, DBSCAN, etc.).
- The CSV file may be replaced with other datasets – just update the loading cell accordingly.

---

By reading through the notebook, you can follow the full workflow used to build and evaluate the customer segmentation model using hierarchical clustering. Enjoy exploring and modifying the analysis!

