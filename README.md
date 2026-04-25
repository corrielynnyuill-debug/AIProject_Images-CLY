# AIProject_Images-CLY
AI Project Unsupervised Image Clustering and Visualization using MNIST

# **MNIST Unsupervised Learning: K‑Means, PCA, and t‑SNE**

This project applies unsupervised learning techniques to the MNIST dataset of handwritten digits. The goal is to explore how clustering and dimensionality reduction can reveal structure in high‑dimensional image data **without using labels**.

---

## **Project Overview**

The workflow includes:

- **Data Loading & Preprocessing**  
  - Loaded MNIST using TensorFlow  
  - Flattened 28×28 images into 784‑dimensional vectors  
  - Normalized pixel values to \([0, 1]\)

- **Clustering with K‑Means**  
  - Used the Elbow Method to select the number of clusters  
  - Trained a K‑Means model on 60,000 training images  
  - Visualized cluster centroids as “average digits”

- **Model Evaluation**  
  - Predicted cluster assignments for test images  
  - Compared clusters to true labels using a cross‑tab  
  - Computed a pseudo‑accuracy by mapping clusters to digits

- **Dimensionality Reduction & Visualization**  
  - Applied PCA (2D) for global structure  
  - Applied t‑SNE (2D) for nonlinear cluster separation  
  - Visualized clusters in reduced space

---

## **Technologies Used**

- Python  
- TensorFlow / Keras  
- Scikit‑learn  
- NumPy  
- Matplotlib / Seaborn  

---

## **Key Findings**

- K‑Means discovers meaningful digit groupings despite no labels  
- Cluster centroids resemble recognizable digits  
- PCA provides broad structure; t‑SNE reveals tight clusters  
- Pseudo‑accuracy typically falls around **55–65%**, reasonable for unsupervised learning
