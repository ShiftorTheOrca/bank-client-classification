# Bank Transaction Clustering & Classification

**NOTE: THIS README FILE IS AI GENERATED.**

This project is a submission for a machine learning module by **Dicoding Indonesia**. Main structures and template are made by the Dicoding. 
This project contains a machine learning workflow for analyzing bank transaction data using both **Clustering** and **Classification** techniques. 

The work was completed as part of the BMLP final submission and consists of two main stages:

1. **Customer/Transaction Segmentation (Clustering)**
2. **Cluster Prediction (Classification)**

## Project Structure

```
.
├── [Clustering]_Submission_Akhir_BMLP_Leonardo_Sanjaya.ipynb
├── [Klasifikasi]_Submission_Akhir_BMLP_Leonardo_Sanjaya.ipynb
├── data_clustering.csv
├── data_clustering_inverse.csv
├── model_clustering.h5
├── PCA_model_clustering.h5
├── decision_tree_model.h5
├── explore_knn_classification.h5
├── explore_random_forest_classification.h5
└── tuning_classification.h5
```

## Dataset

The dataset contains financial transaction records and customer information, including:

- Transaction amount
- Transaction duration
- Account balance
- Customer age
- Occupation
- Login attempts
- Transaction dates
- Other transaction-related attributes

The dataset is suitable for:

- Customer segmentation
- Fraud and anomaly analysis
- Behavioral pattern discovery
- Predictive modeling

## Clustering Stage

### Objectives

Group transactions/customers with similar characteristics using unsupervised learning.

### Workflow

1. Load and inspect dataset
2. Perform data cleaning
3. Encode categorical features
4. Scale numerical features using MinMaxScaler
5. Determine optimal number of clusters using Elbow Method
6. Train K-Means clustering model
7. Evaluate clustering quality using Silhouette Score
8. Visualize cluster distributions
9. Perform PCA-based clustering comparison
10. Interpret cluster characteristics

### Algorithms & Libraries

- K-Means Clustering
- PCA (Principal Component Analysis)
- KElbowVisualizer
- Silhouette Score

### Outputs

- `model_clustering.h5`
- `PCA_model_clustering.h5`
- `data_clustering.csv`
- `data_clustering_inverse.csv`

---

## Classification Stage

### Objectives

Predict cluster labels generated from the clustering process.

### Workflow

1. Load clustering output dataset
2. Preprocess features
3. Split data into training and testing sets
4. Train classification models
5. Evaluate model performance
6. Perform hyperparameter tuning
7. Save trained models

### Algorithms

- Decision Tree Classifier
- K-Nearest Neighbors (KNN)
- Random Forest Classifier

### Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score

### Outputs

- `decision_tree_model.h5`
- `explore_knn_classification.h5`
- `explore_random_forest_classification.h5`
- `tuning_classification.h5`

---

## Requirements

Main libraries used:

```bash
numpy
pandas
matplotlib
seaborn
scikit-learn
yellowbrick
joblib
```

Install dependencies:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn yellowbrick joblib
```

## Running the Project

### Clustering

Open and run:

```bash
[Clustering]_Submission_Akhir_BMLP_Leonardo_Sanjaya.ipynb
```

This notebook will generate cluster labels and export the processed dataset.

### Classification

After the clustering stage is completed, open and run:

```bash
[Klasifikasi]_Submission_Akhir_BMLP_Leonardo_Sanjaya.ipynb
```

This notebook trains classification models using the generated cluster labels as the target.

## Results

The project successfully:

- Segments transaction/customer data using K-Means clustering
- Evaluates cluster quality using Silhouette Score
- Interprets behavioral patterns within each cluster
- Trains multiple classification models to predict cluster membership
- Compares model performance using common classification metrics

## Author

**Leonardo Sanjaya**
