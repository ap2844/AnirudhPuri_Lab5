# AnirudhPuri_Lab5
# Machine Learning and Pattern Recognition  
## Lab 5 – Spring Semester 2026

## Aim
The objective of this lab is to detect faces in an image, extract simple color-based features from the detected faces, cluster them using K-Means, and classify a template face into one of the identified clusters.

## Methodology
1. **Face Detection:**  
   Haar Cascade Classifier (OpenCV) was used to detect faces in the given image.

2. **Feature Extraction:**  
   Each detected face was converted to HSV color space. The mean Hue and Saturation values were computed to form a 2D feature vector for each face.

3. **Clustering:**  
   K-Means clustering was applied to the (Hue, Saturation) feature vectors to group faces into clusters.

4. **Template Classification:**  
   The template image (Dr_Shashi_Tharoor.jpg) was processed in the same way. Its HSV features were extracted and the trained K-Means model was used to predict its cluster label.

## Key Observations
- Faces were grouped based on color characteristics rather than identity.
- The template image was assigned to the cluster whose centroid was closest in feature space.
- The value of K influences clustering behavior and cluster separation.

## Conclusion
This lab demonstrates how basic color features combined with K-Means clustering can be used to group similar faces. It highlights the importance of feature selection and shows how clustering can be applied for simple image-based classification tasks.
