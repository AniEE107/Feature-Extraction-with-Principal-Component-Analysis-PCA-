# Feature-Extraction-with-Principal-Component-Analysis-PCA-
This Jupyter Notebook demonstrates Principal Component Analysis (PCA) for feature extraction. It visualizes synthetic 3D data, then applies PCA to reduce dimensionality to 2D, showcasing how PCA can simplify complex data while preserving class separability.

#  Overview & Purpose
This Jupyter Notebook provides a practical demonstration of Principal Component Analysis (PCA), a fundamental technique in feature extraction and dimensionality reduction. In many real-world datasets, features can be highly correlated or redundant, leading to increased computational cost and potentially hindering model performance. PCA transforms the original features into a new set of uncorrelated variables called principal components, which capture the maximum variance in the data.

# The primary purpose of this notebook is to:
Illustrate PCA Concepts: Clearly show the steps involved in PCA, from data standardization to calculating covariance matrices, eigenvalues, and eigenvectors.
Dimensionality Reduction: Demonstrate how PCA can reduce the number of features while retaining most of the important information.
Visualizing High-Dimensional Data: Show how PCA enables the visualization of data that originally exists in higher dimensions (e.g., 3D data projected to 2D).
Class Separability: Highlight how PCA can preserve or even enhance the separability of different classes in the transformed lower-dimensional space.

#  Key Concepts & Functionality
The notebook covers the following aspects of PCA and feature extraction:
Synthetic Data Generation: Creates a 3D dataset with two distinct classes using numpy.random.multivariate_normal, allowing for a controlled environment to demonstrate PCA.
3D Visualization (Plotly): Uses plotly.express to create an interactive 3D scatter plot of the original data, enabling visualization of the class separation in the original feature space.
Standardization (Mean Centering): Applies StandardScaler from sklearn.preprocessing to standardize the features, a crucial prerequisite for PCA.
Covariance Matrix Calculation: Computes the covariance matrix of the scaled data, which is essential for identifying the relationships between features.
Eigenvalues and Eigenvectors: Calculates the eigenvalues and eigenvectors of the covariance matrix. Eigenvectors represent the principal components, and eigenvalues represent the amount of variance explained by each component.
Dimensionality Reduction: Selects the top principal components based on their explained variance.
2D Visualization of PCA Results: Projects the data onto the chosen principal components and visualizes the transformed data in a 2D scatter plot using plotly.express, demonstrating the effectiveness of the reduction.

#  Technologies Used
Python
Pandas (for data manipulation)
NumPy (for numerical operations, especially for generating synthetic data and linear algebra for PCA)
Scikit-learn (StandardScaler for preprocessing)
Plotly Express (for interactive 3D and 2D visualizations)
Matplotlib (for basic plotting, potentially for visualizing eigenvectors)
Jupyter Notebook
