# Machine Learning and Pattern Recognition  
## Lab 5 – Face Detection and KMeans-Based Face Grouping  

**Author:** Ayushmaan  
**ID:** U20240117

---

## Overview

This lab explores the combination of classical computer vision techniques and unsupervised learning methods. The project focuses on detecting faces in images, extracting meaningful color-based features, and applying KMeans clustering to group similar faces. A template-based approach is also used to classify a new face into an existing cluster.

---

## Objectives

The main goals of this lab are:

- Detect human faces using a pre-trained Haar Cascade classifier  
- Extract HSV color features from detected faces  
- Apply KMeans clustering to group faces based on similarity  
- Classify a template face using cluster centroids  
- Visualize clustering results in a 2D feature space  

---

## Experimental Procedure

### 1. Face Detection

A Haar Cascade face detector was applied to:

- A group faculty image  
- A reference template image  

All visible faces in the group image were successfully identified.

---

### 2. Feature Extraction

For each detected face:

- The face region was cropped  
- The image was converted from BGR to HSV color space  
- Mean Hue and Mean Saturation values were calculated  

Each face was represented as a two-dimensional feature vector:

- X-axis: Hue  
- Y-axis: Saturation  

This provided a compact and interpretable representation of facial color characteristics.

---

### 3. KMeans Clustering

- KMeans was applied with **k = 2**  
- Faces were divided into two clusters based on HSV features  
- Cluster centroids were computed and visualized  

This allowed grouping faces according to similarity in color distribution.

---

### 4. Template-Based Classification

The template face underwent the same preprocessing and feature extraction steps.

- Its Hue and Saturation values were computed  
- The feature vector was projected into the same 2D space  
- The template was assigned to the nearest cluster using centroid distance  

---

## Results and Visualizations

- **Face Detection:** 30 faces were detected in the group image  
- **Feature Plot:** All faces were visualized in a 2D Hue-Saturation space  
- **Cluster Visualization:** Two distinct clusters were observed  
- **Template Projection:** The template face was correctly mapped into one of the clusters  

Plots included:

- Face detection outputs  
- 2D feature distribution  
- KMeans clustering with centroids  
- Final classification including template face  

---

## Key Observations

- Haar Cascade reliably detected faces in both images.
  ![detected_faces](https://github.com/user-attachments/assets/a9c23275-1a87-484b-84c1-54a3e77a147e)
 
  
- HSV color features provided a simple yet effective low-dimensional representation.
- <img width="1005" height="545" alt="image" src="https://github.com/user-attachments/assets/8b996e78-a917-41ea-880f-72526adaa232" />

- KMeans successfully separated faces into two visually meaningful groups.
<img width="1005" height="545" alt="image" src="https://github.com/user-attachments/assets/c1cf9f02-74c9-4d54-824e-a978cf34195a" />

- The template classification demonstrated how new samples can be assigned using centroid distance.
<img width="1005" height="545" alt="image" src="https://github.com/user-attachments/assets/294b0143-441b-41e7-8c6f-b1a1d2881910" />

- 2D visualization improved interpretability of clustering behavior.  
<img width="1005" height="545" alt="image" src="https://github.com/user-attachments/assets/03a0e6f8-ac50-4345-9661-698887e53713" />

---

## Conclusion

This lab demonstrates how traditional computer vision methods can be integrated with unsupervised learning techniques for basic facial grouping tasks. By using HSV-based feature extraction and KMeans clustering, faces were grouped based on color similarity in a reduced feature space. The template classification step further illustrated how new inputs can be mapped into existing clusters using distance-based assignment.

---

## Tools and Libraries Used

- Python  
- OpenCV  
- NumPy  
- Matplotlib  
- scikit-learn  

---
