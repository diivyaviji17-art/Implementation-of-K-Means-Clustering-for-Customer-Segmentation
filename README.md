# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: R.Divyadharshini
RegisterNumber: 212225230062
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.cluster import KMeans

# Load dataset
data = pd.read_csv("Mall_Customers.csv")

# Select features
X = data[['Annual Income (k$)', 'Spending Score (1-100)']]

# Display first few rows
print(data.head())

# Apply K-Means
kmeans = KMeans(n_clusters=5, random_state=42)
y_kmeans = kmeans.fit_predict(X)

# Add cluster column
data['Cluster'] = y_kmeans

# Print clustered data
print("\nClustered Data:")
print(data.head())

# Plot clusters
plt.figure()

plt.scatter(X[y_kmeans == 0]['Annual Income (k$)'],
            X[y_kmeans == 0]['Spending Score (1-100)'],
            label='Cluster 0')

plt.scatter(X[y_kmeans == 1]['Annual Income (k$)'],
            X[y_kmeans == 1]['Spending Score (1-100)'],
            label='Cluster 1')

plt.scatter(X[y_kmeans == 2]['Annual Income (k$)'],
            X[y_kmeans == 2]['Spending Score (1-100)'],
            label='Cluster 2')

plt.scatter(X[y_kmeans == 3]['Annual Income (k$)'],
            X[y_kmeans == 3]['Spending Score (1-100)'],
            label='Cluster 3')

plt.scatter(X[y_kmeans == 4]['Annual Income (k$)'],
            X[y_kmeans == 4]['Spending Score (1-100)'],
            label='Cluster 4')

# Plot centroids
plt.scatter(kmeans.cluster_centers_[:, 0],
            kmeans.cluster_centers_[:, 1],
            s=200, label='Centroids')

# Labels and title
plt.title("Customer Segmentation using K-Means")
plt.xlabel("Annual Income (k$)")
plt.ylabel("Spending Score (1-100)")

plt.legend()
plt.show() 
*/
```

## Output:
<img width="978" height="438" alt="Screenshot 2026-03-19 121131" src="https://github.com/user-attachments/assets/d830e2e2-7475-4d47-9649-b4331a26094e" />
<img width="733" height="437" alt="Screenshot 2026-03-19 121145" src="https://github.com/user-attachments/assets/0026cf78-1cfa-44aa-9cbd-98f679b9d99a" />



## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
