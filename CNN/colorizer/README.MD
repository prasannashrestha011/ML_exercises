
# Deep Learning-Based Image Colorization Using LAB CNNs



---

## Overview
This project implements a convolutional neural network (CNN) to colorize grayscale images using the **LAB color space**. The model takes the L (lightness) channel as input and predicts the ab channels. Predicted channels are combined with L to reconstruct the color image. The approach is trained on the **Caltech101 dataset** and is optimized for medium-scale datasets and Colab environments.

---

## Features
- Automatic colorization of grayscale images  
- LAB color space-based prediction for better perceptual quality  
- Lightweight CNN suitable for Colab GPU  
- Interactive prediction for user-uploaded images  

---

## Dataset
- **Dataset:** Caltech101 (or Caltech256)  
- **Number of images:** ~9,000 images (Caltech101)  
- **Preprocessing steps:**  
  1. Resize images to 128×128  
  2. Discard alpha channel if present (RGBA → RGB)  
  3. Scale L channel to `[0,1]`  
  4. Scale ab channels to `[-1,1]`  

---
!(colorizer results)[../images/colorizer.png]

