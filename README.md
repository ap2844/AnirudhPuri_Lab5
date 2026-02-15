## Aim
The aim of this lab is to detect faces in an image, extract simple color features from the detected faces, cluster them using K-Means, and classify a separate template image based on those clusters.

## Methodology
First the faces were detected using the Haar Cascade classifier in OpenCV and each detected face was converted to HSV color space, and the mean Hue and Saturation values were calculated to form a feature vector. Then K-Means clustering was applied to group faces based on these features. And finally, the same feature extraction process was applied to the template image, and its cluster label was predicted using the trained K-Means model.

## Observations
The clustering grouped faces based on overall color characteristics like hue and saturation rather than identity. The template image was assigned to the cluster whose centroid was closest in the feature space.

## Conclusion
This experiment demonstrates how simple feature extraction combined with K-Means clustering can be used for basic grouping and classification tasks in image processing.
