# Titanic Cluster Analysis

Unsupervised machine learning project using K-Means clustering to discover natural passenger groups in the Titanic dataset. The analysis identifies 3 distinct passenger segments based on features like class, fare, gender, and embarkation port.

## Overview

This notebook explores whether Titanic passengers can be grouped into meaningful clusters without using survival information. The goal is to discover hidden patterns and passenger segments that existed aboard the ship.

## Results

**Optimal Clusters:** 3 passenger groups

**Performance Metrics:**
- Silhouette Score: **0.523** (good separation, scale -1 to 1)
- Davies-Bouldin Index: **0.785** (low similarity between clusters, lower is better)
- Calinski-Harabasz Index: **863.51** (high density and separation, higher is better)

**Cluster Interpretation:**
- **Cluster 0:** Higher-class passengers with elevated fares
- **Cluster 1:** Lower-class passengers with minimal fares  
- **Cluster 2:** Mixed demographic with moderate characteristics

The clusters align with socioeconomic stratification aboard the Titanic, showing that class and fare were dominant factors in passenger grouping.

## Prerequisites

**Required Libraries:**
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## How to Run

1. **Download** `TitanicClusterAnalysis.ipynb` from this repository

2. **Get the Dataset:**
   - Download from [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)
   - Save the file as `titanic_dataset.csv`

3. **Open in Google Colab:**
   - Go to [Google Colab](https://colab.research.google.com/)
   - Upload the notebook (File → Upload notebook)
   - Upload `titanic_dataset.csv` (click folder icon → upload)
   - Run all cells (Runtime → Run all)

## What's Inside

**1. Exploratory Data Analysis**  
Examines dataset structure, distributions, and relationships between variables.

**2. Data Preprocessing**  
Handles missing values, creates new features (FamilySize), encodes categorical variables, and standardizes numerical features.

**3. Optimal Cluster Selection**  
Uses the Elbow Method to determine the best number of clusters (k=3).

**4. K-Means Clustering**  
Groups passengers into 3 clusters and analyzes their composition.

**5. Visualization**  
Uses PCA to reduce dimensions and visualize clusters in 2D space.

**6. Evaluation**  
Measures cluster quality using Silhouette Score, Davies-Bouldin Index, and Calinski-Harabasz Index.

## Key Insights

- Passengers naturally segment into 3 groups based on socioeconomic factors
- Class and fare are the strongest differentiators
- Clusters show clear separation with minimal overlap
- These groupings likely influenced survival rates due to cabin location and lifeboat access

## Author Contact

**Hashim Choudhry**  
- GitHub: [@h4hash-ch](https://github.com/h4hash-ch)
- Linkedin: [Connect with me](https://www.linkedin.com/in/hashim-choudhry)
