# Image Stitching using Harris, SIFT, and RANSAC

This project implements an **image stitching pipeline** in Python using OpenCV.  
It merges two overlapping images into a single panoramic view by detecting, matching, and aligning keypoints.

---

## Overview
The system compares two feature detection methods:
- **Harris Corner Detector** (with patch-based descriptors)  
- **SIFT (Scale-Invariant Feature Transform)** for scale and rotation invariance  

A **custom RANSAC-based affine transformation estimator** is used to filter outliers and achieve accurate alignment.  
Finally, a **distance-weighted blending** method ensures smooth transitions between overlapping regions.

---

## Features
- Harris and SIFT keypoint detection  
- Brute-force descriptor matching  
- Custom RANSAC for affine transformation  
- Image warping and blending  
- Sensitivity analysis (thresholds & top matches)

---

## Technologies Used
- Python  
- OpenCV  
- NumPy  
- Matplotlib  
