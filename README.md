# 🏍️ Bike Image Classification Using HOG Features and K-Means

## 📌 Project Overview
This project uses Computer Vision and Unsupervised Machine Learning to group similar-looking bike images using HOG (Histogram of Oriented Gradients) feature extraction and the K-Means clustering algorithm.

The system analyzes bike images based on their shapes and edge patterns and automatically groups them into different clusters without requiring predefined image labels.

## 🎯 Project Objectives
- Load and preprocess bike images.
- Extract image features using HOG.
- Reduce feature dimensions using PCA.
- Group similar images using K-Means clustering.
- Visualize the generated clusters.
- Predict the cluster of a new bike image.

## 🛠️ Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-image
- Scikit-learn
- Pillow
- Jupyter Notebook

## 🧠 Machine Learning Techniques

### 1. HOG (Histogram of Oriented Gradients)
Extracts important shape and edge information from bike images.

### 2. StandardScaler
Scales extracted features to a similar range.

### 3. PCA (Principal Component Analysis)
Reduces 8,100 HOG features to 50 principal components.

### 4. K-Means Clustering
Groups similar bike images into 5 clusters.

### 5. Model Evaluation
Uses:
- Elbow Method
- Silhouette Score
- Inertia

## ⚙️ Project Workflow
1. Load bike image dataset.
2. Resize images to 128 × 128 pixels.
3. Convert images into grayscale.
4. Extract HOG features.
5. Apply feature scaling.
6. Reduce dimensions using PCA.
7. Select the number of clusters using evaluation techniques.
8. Apply K-Means clustering.
9. Visualize similar bike images.
10. Save clustered images into separate folders.
11. Predict the cluster of a new bike image.

## 📂 Project Structure

```text
Bike-Image-Classification/
│
├── Bike_Image_Classification_HOG_Kmeans.ipynb
├── README.md
├── requirements.txt
│
└── bike_clusters/
    ├── cluster_0/
    ├── cluster_1/
    ├── cluster_2/
    ├── cluster_3/
    ├── cluster_4/
    └── cluster_assignments.csv
```

## 📊 Dataset Information
- Total images: 209 (as described in the notebook).
- Image types: Bicycle, Scooter, Motorcycle and E-bike photos.
- Image size: 128 × 128 pixels.
- Image format: JPG, JPEG, PNG, WEBP and BMP.

## 📈 Results
- Extracted 8,100 HOG features per image.
- Reduced the features to 50 using PCA.
- Grouped images into 5 clusters using K-Means.
- Visualized the generated clusters.
- Saved the cluster assignments in a CSV file.
- Created a function to assign a new bike image to a cluster.

Note: The clusters represent visual similarity, not verified vehicle categories.

## 🚀 How to Run the Project

### Step 1: Clone the repository
```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### Step 2: Install dependencies
```bash
pip install numpy pandas matplotlib scikit-image scikit-learn Pillow
```

### Step 3: Open Jupyter Notebook
```bash
jupyter notebook
```

### Step 4: Update the image folder path
Set `IMAGE_FOLDER` in the notebook to your local bike image dataset location.

### Step 5: Run the notebook
Execute all cells to extract features, perform clustering and visualize the results.

## 🔮 Future Improvements
- Improve image grouping using deep learning.
- Experiment with different clustering algorithms.
- Increase dataset size.
- Compare HOG features with CNN-based image features.
- Evaluate clustering quality with additional metrics.

Mechanical Engineering Graduate | Aspiring Machine Learning Engineer

Skills: Python | Machine Learning | Deep Learning | Computer Vision | Data Analysis

## ⭐ Conclusion
This project demonstrates how Computer Vision and Unsupervised Machine Learning can be combined to extract image features and automatically group visually similar bike images.
