# Medical-Healthcare-Assistance-System

This Streamlit web application provides a unified platform for disease prediction and recommendations based on user input. The app supports four distinct modules:
- Symptom-Based Disease Prediction
- Diabetes Prediction
- Breast Cancer Prediction
- MRI Tumor Detection

---

## Features

- **Intuitive Navigation:** Choose from four health prediction services in the sidebar.
- **Multi-Modal Inputs:** Use text, dropdowns, form fields, or images as appropriate for each type of prediction.
- **Instant Recommendations:** Provides precautions, medications, diet, and workout tips for predicted diseases (where supported).
- **AI-Powered:** Employs machine learning models (Sklearn & TensorFlow/Keras) for accurate classification and prediction.

---

## Usage Overview

### 1. Symptom-Based Disease Prediction

- Select symptoms from the provided checklist.
- Click "Predict".
- View most probable disease, its description, precautions, medications, diet, and recommended workouts.

### 2. Diabetes Prediction

- Enter values for medical features (pregnancies, glucose, blood pressure, etc.).
- Click "Predict Diabetes" to see whether you are likely to have diabetes.

### 3. Breast Cancer Prediction

- Input values for the listed clinical features.
- Click "Predict Breast Cancer" for a diagnosis (Malignant/Benign).

### 4. MRI Tumor Detection

- Upload an MRI image (`.jpg`, `.jpeg`, or `.png`).
- The app predicts if the scan indicates "No Tumor" or the tumor type.
- Displays prediction and confidence score.

---

## Key Technological Details

- **Framework:** [Streamlit](https://streamlit.io/)
- **Backends Used:** `joblib` for Sklearn models, TensorFlow/Keras for deep learning, `cosine_similarity` from scikit-learn for symptom matching.
- **File Handling:** Models and datasets are read dynamically from specified directories; errors are handled gracefully if files are missing.

---

## Notes

- All models must be present in the `models` folder for their respective modules to work.
- CSV datasets should stay inside the `datasets` folder.
- Modify supported symptoms/diseases or add new ones by updating the CSVs.


