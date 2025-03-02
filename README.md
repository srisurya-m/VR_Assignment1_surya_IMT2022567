# VR Assignment 1

## Author: Surya

## Overview
This repository contains the implementation of VR Assignment 1, which includes two tasks:
1. **Coin Detection, Segmentation, and Counting** – Detecting, segmenting, and counting Indian coins using computer vision techniques.
2. **Image Stitching for Panorama Creation** – Creating a stitched panorama from multiple overlapping images.

## Part 1: Coin Detection, Segmentation, and Counting
### Objective
- Detect coins in an image using edge detection.
- Segment individual coins from the background.
- Count the total number of coins.

### Approach
1. **Coin Detection**
   - Applied Canny edge detection and contour detection to locate coins.
   - Outlined detected coins on the input image.

2. **Segmentation**
   - Used thresholding and morphological operations to isolate coins.
   - Extracted each segmented coin separately.

3. **Counting**
   - Counted the number of detected coin contours.
   - Displayed the total count on the processed image.

### Results
- The results, including detected coins, segmented images, and total coin count, are available in `main_coin.ipynb`.

## Part 2: Image Stitching for Panorama Creation
### Objective
- Detect key points in overlapping images.
- Use feature matching to align images.
- Stitch images into a panorama.

### Approach
1. **Keypoint Detection**
   - Used SIFT/ORB/SURF to extract keypoints.
   - Matched keypoints between images using feature matching algorithms.

2. **Image Stitching**
   - Computed homography transformation for alignment.
   - Warped and blended images to form a panoramic output.

### Results
- The results, including keypoint detection, feature matching, and the final stitched panorama, are available in `main_image_stitch.py`.

## Installation & Requirements
Install dependencies using:
pip install opencv-python numpy scikit-image matplotlib

## Repository Structure
VR_Assignment1_surya_IMT2022567/
│-- part-1/
│   │-- coin_detector.ipynb  # Jupyter Notebook for Coin Detection
│   │-- coins.jpg            # Input image for coin detection
│-- part-2/
│   │-- image_stitcher.py    # Python script for Image Stitching
│   │-- panorama1.jpeg       # First input image
│   │-- panorama2.jpeg       # Second input image
│-- report.pdf               # Detailed explanation of the methods used
│-- README.md                # Project Documentation

