# Cluster-Analysis-of-Online-Food-Delivery-Popularity-Through-Uber
Utilising clustering algorithms like Affinity Propagation, Gaussian Mixture Models, Spectral Clustering, Fuzzy C-means, and Hierarchical Clustering to reveal  customer segments and patterns in Uber Eats USA data, generating practical suggestions and visual insights.

## Table Of Contents
- [Introduction](#introduction)
- [Usage](#usage)
- [Dashboard](#dashboard)
- [Methodology](#methodology)
- [Results](#results)
- [License](#license)
- [References](#references)

## Introduction
This project utilises Spectral Clustering, Fuzzy C-means, and Hierarchical Clustering to uncover customer segments and insights within Uber Eats USA data, driving strategic recommendations.

## Usage
To run the clustering analysis, follow these steps:

1. Ensure you have Jupyter Notebook installed. If not, you can install it using:
    ```bash
    pip install notebook
    ```

2. Navigate to the project directory where the Jupyter Notebook is located:
    ```bash
    cd ClusterAnalysisOfUberEats
    ```

3. Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

4. In the Jupyter Notebook interface, open the `UberEatsClusterAnalysis.ipynb` file.

5. Download the two datasets from [Uber Eats USA](https://www.kaggle.com/datasets/ahmedshahriarsakib/uber-eats-usa-restaurants-menus?select=restaurants.csv) and rename them as `restaurants.csv` and `restaurant-menus.csv`. Place the files in the same directory as the Jupyter Notebook.

6. Run the cells in the notebook to execute the clustering analysis.

## Dashboard
A simple dashboard has been created using Streamlit to visualize the clustering results.

The code for the dashboard and the CSV files containing the results are located in the `Dashboard` folder within this repository.

## Methodology

The project utilises the Uber Eats USA dataset. It applies Affinity Propagation, Fuzzy C-Means, Hierarchical Clustering, Spectral Clustering, and Gaussian Mixture Models to cluster restaurant segments, following preprocessing steps like missing value handling, data validation, and outlier removal.

### Data Collection

- **Source:** Uber Eats USA dataset available on [Uber Eats USA]([https://world.openfoodfacts.org/data](https://www.kaggle.com/datasets/ahmedshahriarsakib/uber-eats-usa-restaurants-menus?select=restaurants.csv))
- **Size:** 10MB/ 63k+ and 11 columns

### Clustering Algorithms

1. **Affinity Propagation:** Clusters data by identifying exemplars without needing a predefined number of clusters.
2. **Fuzzy C-Means:** Forms overlapping clusters, allowing data points to have varying degrees of membership.
3. **Hierarchical Clustering:** Builds a tree-like hierarchy of clusters, useful for creating clusters at multiple levels.
4. **Spectral Clustering:** Uses eigenvalues of a similarity matrix for dimensionality reduction before clustering.
5. **Gaussian Mixture Models:** Models data as a mixture of Gaussian distributions, assigning points to clusters probabilistically.

## Results

Clustering results reveal insights into data patterns and relationships, helping better understand to the dataset. 

- **Affinity Propagation:** Shows moderate cluster definition, with the Silhouette Score(0.3301) indicating some overlap but generally distinct clustering.
- **Fuzzy C-Means:** Has the lowest Silhouette Score(0.2826), indicating the most cluster overlap.
- **Spectral Clustering:** Achieves the highest Silhouette Score(0.6524), indicating the most distinct and well-defined clusters.
- **Gaussian Mixture Models:** Achieves a moderate Silhouette Score(0.3150), with GMM clusters showing some overlap.
- **Hierarchical Clustering:** Hierarchical Clustering’s Silhouette Score(0.3110) indicates moderate cluster definition with some overlap.
  
In this project, the most suitable clustering method is spectral clustering. This is due to its ability to handle complex data structures and identify non-linear relationships in the data, which other algorithms may miss.

## License

This project forms part of an academic course and is intended solely for educational purposes. It may include references to copyrighted materials and any such materials are utilised exclusively for scholarly use. For guidance on sharing or distributing this work, it is advisable to seek consultation from your instructor or institution.

For more details, see the [LICENSE](./LICENSE.txt) file.

## Reference
**Dataset:** [Uber Eats USA](https://www.kaggle.com/datasets/ahmedshahriarsakib/uber-eats-usa-restaurants-menus?select=restaurants.csv)
