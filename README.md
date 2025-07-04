#  Sound Clustering Assignment

This notebook demonstrates the process of unsupervised clustering on unlabeled sound data using machine learning techniques, with a focus on feature extraction, dimensionality reduction, and clustering evaluation.

---

##  Dataset

- The dataset consists of `.wav` files stored in a specified directory.
- Mel spectrograms were extracted as features using the `librosa` library.

---

##  Objectives

1. Extract meaningful features from raw sound files.
2. Scale and standardize the extracted features.
3. Apply dimensionality reduction (PCA, t-SNE).
4. Perform clustering (K-Means, DBSCAN).
5. Evaluate and visualize the clustering results.
6. Analyze the effectiveness of each method.

---

##  Methods Used

###  Feature Extraction
- **Librosa's Mel spectrogram**: Computes frequency features from each audio file.

###  Preprocessing
- **StandardScaler**: Standardizes features to have zero mean and unit variance.

###  Dimensionality Reduction
- **PCA (Principal Component Analysis)**: Captures global variance with fewer dimensions.
- **t-SNE (t-distributed Stochastic Neighbor Embedding)**: Preserves local similarities for better visualization.

### Clustering Algorithms
- **K-Means**: Partitioning method based on minimizing intra-cluster distances.
- **DBSCAN**: Density-based method that handles noise and finds arbitrarily shaped clusters.

---

## Key Observations

- Dimensionality reduction made high-dimensional data interpretable and improved clustering performance.
- t-SNE provided better cluster separability than PCA in visualizations.
- K-Means worked well for compact clusters; DBSCAN was better at identifying noise and irregular structures.
- Clustering results were visualized in 2D/3D for interpretation.

---

## Final Analysis

- Dimensionality reduction revealed structure in data and improved clustering outcomes.
- K-Means required prior knowledge of cluster count but gave stable results.
- DBSCAN excelled in handling noisy data without needing a fixed number of clusters.
- The project reflects real-world challenges in audio analytics, where data is complex and label-free.

---

## ▶️ How to Run

1. Mount your Google Drive.
2. Update the path to your unlabelled `.wav` files.
3. Run all cells sequentially.

---

##  Dependencies

- `librosa`
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

Install missing libraries via:

```bash
pip install librosa pandas matplotlib seaborn scikit-learn

