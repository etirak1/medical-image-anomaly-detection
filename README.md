# Medical Image Anomaly Detection & Pattern Recognition

This repository contains an end-to-end computer vision and image processing pipeline designed to detect, localize, and analyze structural anomalies in medical scans (e.g., MRI, CT, or X-ray imaging). 

The project applies classical digital image processing techniques alongside modern machine learning approaches to perform noise suppression, contrast enhancement, region segmentation, and anomaly classification.

---

## 📌 Project Overview & Pipeline

Medical imaging requires high precision and robustness to assist clinical diagnosis. This pipeline is divided into four modular stages:

1. **Preprocessing & Artifact Removal:**
   * Spatial filtering (Gaussian, Median filter) for high-frequency noise suppression.
   * Contrast Limited Adaptive Histogram Equalization (**CLAHE**) for local contrast improvement.
   * Intensity normalization and skull stripping / region-of-interest (ROI) isolation.

2. **Feature Extraction & Morphological Analysis:**
   * Edge detection using Canny and Sobel gradient operators.
   * Morphological transformations (Dilation, Erosion, Opening, Closing) to refine segment boundaries.
   * Contour extraction and shape/texture descriptor computation.

3. **Anomaly Detection & Segmentation:**
   * Thresholding-based segmentation (Otsu's method / Adaptive Thresholding).
   * Machine learning / deep learning classification to distinguish pathological regions from healthy tissue.
   * Bounding-box localization and contour masking of identified anomalies.

4. **Visualization & Diagnostic Reporting:**
   * Side-by-side comparative plots (Raw scan vs. Preprocessed vs. Segmented Mask).
   * Visual overlays pinpointing detected anomalous regions.

---

## 🛠️ Tech Stack & Dependencies

* **Language:** Python 3.8+
* **Computer Vision:** OpenCV (`cv2`), Scikit-image (`skimage`)
* **Scientific Computing:** NumPy, SciPy
* **Modeling & Machine Learning:** Scikit-learn, PyTorch / TensorFlow
* **Visualization:** Matplotlib, Seaborn

---


## 🚀 Getting Started

### 1. Clone the repository:
```bash
git clone https://github.com/etirak1/medical-image-anomaly-detection.git
cd medical-image-anomaly-detection


---

## 👥 Contributors

This project was collaboratively developed by:

* Ali Ljaljak
* Elma Tirak
* Amina Kazazović
* Daris Mujkić
* Benjamin Hadžihasanović
