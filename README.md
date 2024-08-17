# Skancer - Skin Cancer Detection and Classification

Skancer is an end-to-end machine learning solution developed to enhance the early detection and classification of skin cancer. This project leverages advanced deep learning models like ResNet and EfficientNet to accurately identify and classify various types of skin cancer. The project was developed as part of the GAIP program at NUS Singapore.

## Introduction

Skin cancer is one of the most common types of cancer, and early detection is crucial for effective treatment. Skancer leverages machine learning models to accurately identify and classify various skin cancer types, improving diagnostic accuracy and aiding medical professionals.

## Data Acquisition

This project utilizes the Kaggle API to download and manage the dataset required for skin cancer detection and classification.

### Dataset Acquisition Steps

1. **Kaggle Account**: Ensure you have a Kaggle account. If you don’t have one, you can sign up at [Kaggle](https://www.kaggle.com/).

2. **Kaggle API Token**:
   - Go to your Kaggle account settings and create a new API token. This will download a file named `kaggle.json`.
   - Place the `kaggle.json` file in the root directory of your project.

3. **Download the Dataset**:
   - Use the following commands in your Jupyter notebook or Python script to download the dataset:
   ```bash
   !pip install kaggle
   !mkdir -p ~/.kaggle
   !cp kaggle.json ~/.kaggle/
   !kaggle datasets download -d <dataset-name>
   !unzip <dataset-name>.zip -d data/
!kaggle datasets download -d <dataset-name>
!unzip <dataset-name>.zip -d data/

Replace <dataset-name>: Make sure to replace <dataset-name> with the actual name of the dataset you are using.
By following these instructions, you can easily set up the dataset for the Skancer project.

## Frontend Integration

This project includes an HTML interface for uploading images and displaying results based on the type of skin cancer detected.

### Files Included

- **`frontend/index.html`**: HTML file for image upload.
- **`frontend/Actinic_keratosis.html`**: HTML file for displaying results for Actinic Keratosis.
- **`frontend/Basal_Cell_Carcinoma.html`**: HTML file for displaying results for Basal Cell Carcinoma.
- **`frontend/Dermatofibroma.html`**: HTML file for displaying results for Dermatofibroma.
- **`frontend/Vascular_lesions.html`**: HTML file for displaying results for Vascular Lesions.
- **`frontend/Melanoma.html`**: HTML file for displaying results for Melanoma.
- **`frontend/Benign_keratosis_like_lesions.html`**: HTML file for displaying results for Benign Keratosis-like Lesions.
- **`src/frontend_integration.py`**: Script for handling image uploads and predictions.
- **`models/model.h5`**: The trained model used for predictions.

### Usage Instructions

1. **Open the HTML file in a web browser**:
   - Navigate to `frontend/index.html` in your local file system.

2. **Upload an image using the provided form**.

3. The application will classify the image and redirect to the corresponding HTML file based on the detected skin cancer type:
   - If the image is classified as **Actinic Keratosis**, it will open `Actinic_keratosis.html`.





