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

![Plaksha_Faculty](https://github.com/user-attachments/assets/a945022f-66b9-445c-ac74-4aa908060cba)


<img width="890" height="594" alt="Total number of face detected are 30_screenshot_14 02 2026" src="https://github.com/user-attachments/assets/bb2fb85e-a22d-49dc-a29a-386bcfd9c459" />



![Dr_Shashi_Tharoor](https://github.com/user-attachments/assets/cb7edcc7-cd94-4f1e-8985-75939de2f700)

<img width="400" height="400" alt="Detected Face in Template Image_screenshot_14 02 2026" src="https://github.com/user-attachments/assets/50455c36-22ba-4122-a53c-dda4f7bb1dcf" />


<img width="509" height="277" alt="Plot 1" src="https://github.com/user-attachments/assets/db59c432-7dcf-47ee-9a87-ca06d4456360" />


<img width="509" height="277" alt="Template image cluster plot" src="https://github.com/user-attachments/assets/69720049-02b9-41c6-b78c-899e206b08b0" />

