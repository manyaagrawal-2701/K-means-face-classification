# Face Detection and Clustering using K-Means

# Aim
The objective of this project is to detect human faces from an image using the Haar Cascade face detection technique and group similar faces using the K-Means clustering algorithm. The clustering is performed using color-based features (Hue and Saturation) extracted from the detected face regions in HSV color space.

---

# Methodology

# Image Processing
- The input image is loaded using OpenCV.
- The image is converted from BGR to grayscale format to simplify face detection.
- Haar Cascade Classifier is applied to detect faces.
- Bounding boxes are drawn around detected faces for visualization.

# Feature Extraction
- Each detected face region is converted from BGR to HSV color space.
- Two main features are extracted:
  - Hue (color tone)
  - Saturation (color intensity)
- Mean values of hue and saturation are calculated to represent each face numerically.
- These values are stored for clustering.

# K-Means Clustering
- The extracted feature vectors are used as input to the K-Means algorithm.
- Faces are grouped into clusters based on similarity in color features.
- Scatter plots are generated to visualize cluster separation.
- Cluster centroids are calculated and displayed to represent average characteristics of each group.

# Template Matching and Prediction
- A template image containing a single face is loaded.
- The face is detected and converted into HSV color space.
- Hue and saturation features are extracted in the same way as the dataset.
- The trained K-Means model predicts the cluster label of the template image.
- The template face is plotted along with existing clusters for comparison.

---

# Results / Key Findings
- Faces were successfully detected from the group image using Haar Cascade.
- HSV-based feature extraction captured color characteristics effectively.
- K-Means clustering grouped visually similar faces into distinct clusters.
- Cluster centroids provided clear representation of each group.
- The template image was correctly assigned to the nearest cluster based on feature similarity.

---

# Conclusion
This project demonstrates how computer vision techniques and machine learning algorithms can be combined for face analysis. Haar Cascade efficiently detects faces, while K-Means clustering groups faces based on color similarity using HSV features. The approach shows that simple feature extraction combined with clustering can be effective for basic face grouping and visual pattern analysis.

![image alt][https://github.com/manyaagrawal-2701/K-means-face-classification/blob/1ddb835848c51d71187fbfbe7c2d7e256c00638c/Plaksha_Faculty.jpg]

![image alt][https://github.com/manyaagrawal-2701/K-means-face-classification/blob/21d4ce3f5036f5e6115a1b1c3e50f0f3ec4e3d54/Total%20number%20of%20face%20detected%20are%2030_screenshot_14.02.2026.png]

