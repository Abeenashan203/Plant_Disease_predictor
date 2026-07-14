# Plant_Disease_predictor (streamlit app)
An end-to-end computer vision program build using streamlit,opencv and sci-kit learn detect whether a plant is infected or health.

# ## Project Overview
This project provides an automated ,non destructive pipeline for farmers agricultural experts to evaluate leaf health instantly .instead of using heavy 
deep learnig models.
###  Key Features
*   **Leaf Segmentation:** Utilizes **Otsu's Automatic Thresholding** to intelligently separate
 the foreground leaf from any noisy background (e.g., soil, hands, tables).
*   **Advanced Feature Extraction:** Extracts a robust 16-dimensional feature vector combining:
    *   **Color Moments (12 Features):** Mean, Standard Deviation, and Skewness calculated across
 **HSV** and **Lab** color spaces to capture discoloration and lesions.
    *   **Texture Metrics (4 Features):** Contrast, Homogeneity, Energy, and Correlation calculated
 via **Gray-Level Co-occurrence Matrix (GLCM)** to evaluate leaf surface roughness.
*   **Interactive Web UI:** A sleek, minimal user interface built with **Streamlit** that allows users
 to drag-and-drop leaf images and view immediate diagnostic banners.

## 🛠️ Tech Stack
*   **Frontend Deployment:** Streamlit
*   **Image Processing & CV:** OpenCV (`cv2`), Pillow (`PIL`), Scikit-image (`skimage`)
*   **Machine Learning:** Scikit-learn (`sklearn`), Joblib
*   **Scientific Computing:** NumPy, SciPy
---
## 📦 Project Structure
*   `app.py` - The main Streamlit web application script containing UI configurations and the feature extraction pipeline.
*   `plant_disease_model.joblib` - The pre-trained Random Forest model containing the diagnostic intelligence.
*   `requirements.txt` - Configuration file listing all project dependencies for seamless replication.
---

## 📊 Dataset Availability
The structured dataset used for training this model is larger than 25MB and is hosted externally on Google Drive. 
You can download the dataset directly from the link below:

*   **Dataset File:** `leaf_features.csv` (27.6 MB)
*   **Download Link:** [Click here to download leaf_features.csv from Google Drive](https://drive.google.com/file/d/1CtNjJ6AC9kb2cxoztfGyj_llY6Hhx576/view?usp=sharing)

---
### 1. Prerequisites
Ensure you have Python 3.10 installed on your local machine.

### 2. Installation & Setup
Clone the repository and install the required dependencies:
```bash
# Install dependencies
pip install -r requirements.txt
