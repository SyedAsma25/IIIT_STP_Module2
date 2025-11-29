# 📚 Module 2: Data Exploration & Dimensionality Reduction

This repository contains work from **Module 2** of the AI/ML learning track, covering exploratory data analysis, visualization, and both linear and non-linear dimensionality reduction techniques.

---

## 🔹 Lab 1: Basic Data Visualization

**Objective**  
Explore and understand the dataset using visual analysis techniques.

**Key Concepts & Plots**
- Histograms and distribution plots  
- Scatter plots and pair plots  
- Box plots, violin plots, and swarm plots  
- Correlation heatmaps and joint plots  

**Dataset**  
- **Automobile Dataset (1985 Ward’s Automotive Yearbook)**  
- **Target Variable:** `price`  

**Insights**  
- Identified skewed features and outliers  
- Observed relationships between price and key numerical features  
- Built intuition for feature importance before modeling  

---

## 🔹 Lab 2: Principal Component Analysis (PCA)

**Objective**  
Apply PCA to reduce dimensionality and visualize high-dimensional data.

**Key Steps**
- Standardization of features  
- Covariance matrix computation  
- Eigenvalues and eigenvectors  
- Explained variance ratio and scree plot  
- 2D and 3D PCA visualization  

**Dataset**  
- **Breast Cancer Wisconsin Dataset** (`sklearn.datasets.load_breast_cancer`)

**Key Insights**
- First **2–3 principal components** show clear separability between **benign** and **malignant** classes.  
- About **6–7 components** retain ~**90%** of the total variance, making PCA useful for preprocessing and speeding up models.

---

## 🔹 Lab 3: Manifold Learning with ISOMAP

**Objective**  
Understand non-linear dimensionality reduction through manifold learning and compare it with PCA.

**Concepts Covered**
- Manifolds and locally Euclidean structure  
- Euclidean vs geodesic distance  
- k-nearest neighbors graph construction  
- Shortest-path computation (Dijkstra)  
- Eigen-decomposition of the Gram matrix  

**Datasets**
- Synthetic **S-Curve dataset** (`sklearn.datasets.make_s_curve`)  
- **Labeled Faces in the Wild (LFW)** dataset (`sklearn.datasets.fetch_lfw_people`)

**Key Insights**
- ISOMAP successfully “unrolls” the S-curve into a meaningful 2D embedding.  
- On face images, ISOMAP discovers latent factors like **pose** and **lighting**, showing the power of non-linear methods over PCA for some data types.

---

## 🔹 Lab 4: t-SNE (t-Distributed Stochastic Neighbor Embedding)

**Objective**  
Use t-SNE for visualizing high-dimensional data while preserving local neighborhood structure.

**Concepts Covered**
- High-dimensional similarity (Gaussian-based probabilities)  
- Low-dimensional similarity (Student-t distribution)  
- Kullback–Leibler (KL) divergence as the optimization objective  
- Gradient descent-based optimization  

**Key Hyperparameters**
- `n_components` (typically 2 for visualization)  
- `perplexity` (controls effective number of neighbors)  
- `n_iter` (number of optimization iterations)  
- `method` (`"barnes_hut"` vs `"exact"`)

**Dataset**
- **Handwritten Digits Dataset** (`sklearn.datasets.load_digits`)

**Key Insights**
- t-SNE creates well-separated digit clusters that are easy to interpret visually.  
- Results are sensitive to hyperparameters (especially perplexity) and random initialization, emphasizing the need to experiment with multiple runs.

---

## ⚙️ Technologies & Libraries

| Library       | Purpose                               |
|--------------|----------------------------------------|
| NumPy, Pandas| Numerical computing & data handling    |
| Matplotlib   | Static visualizations                  |
| Seaborn      | Statistical data visualization         |
| Plotly       | Interactive visualizations (2D/3D)     |
| Scikit-learn | PCA, ISOMAP, t-SNE, datasets, scaling  |
| SciPy        | Distance metrics and graph utilities   |

---

## 👤 Author

**Syed Asma**  

