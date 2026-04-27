AI-Based Plant Image Classification System
 Project Overview

This project presents a deep learning-based image classification system designed to analyse plant leaf images. The system uses both a custom Convolutional Neural Network (CNN) and a transfer learning model (MobileNetV2) to classify images into three categories: color, grayscale, and segmented.

In addition to model development, the project includes a Streamlit web application that allows users to upload images and receive real-time predictions with confidence scores. This demonstrates the practical deployment of deep learning models in a user-friendly environment.

 Features
Image classification using CNN and MobileNetV2
Real-time prediction using Streamlit
Model comparison and evaluation (Accuracy, F1-score, Confusion Matrix)
Data preprocessing and augmentation
Scalable and modular pipeline design
📁 Project Structure
project/
│
├── app.py                      # Streamlit application
├── train.py                   # Model training script
├── model.py                   # CNN / MobileNetV2 architecture
├── data_loader.py             # Dataset loading and preprocessing
├── requirements.txt           # Dependencies
├── README.md                  # Project documentation
│
├── models/
│   └── best_model_mobilenetv2.pth
│
├── notebooks/
│   ├── supriya.ipynb
│   ├── abhilasha.ipynb
│   ├── hari.ipynb
│   ├── kalyan.ipynb
│   └── vijaya.ipynb
│
└── sample_images/             # Example images for testing
 Environment Setup
 Step 1: Clone the Repository
git clone <your-repo-link>
cd project
 Step 2: Install Dependencies
pip install -r requirements.txt
 Requirements

Create a requirements.txt file with the following:

torch
torchvision
streamlit
numpy
matplotlib
scikit-learn
Pillow
 How to Run the Project
 1. Train the Model
python train.py
 2. Run the Streamlit Application
streamlit run app.py
 Open in browser:

http://localhost:8501
 Pre-trained Model

The trained model is stored in:

models/best_model_mobilenetv2.pth

 If the file is too large for GitHub, download from:

[Add Google Drive link here]
 Dataset

Dataset used: PlantVillage Dataset

 Download from:

https://www.kaggle.com/datasets/emmarex/plantdisease
 Model Performance
 MobileNetV2
Accuracy: 98.85%
High precision, recall, and F1-score across all classes
 CNN (Baseline)
Accuracy: 98.31%
Slightly lower than MobileNetV2 but strong baseline performance
 Deployment

The project includes a Streamlit web application that allows:

Uploading plant leaf images
Real-time classification
Display of prediction confidence
 #Team Members
Supriya – Model development, evaluation, deployment
Abhilasha – Data preprocessing and augmentation
Hari Krishna – Data pipeline and Streamlit integration
Kalyan Babu – Data validation and visualization
Vijaya Rama Raju – CNN model design
 #Limitations
Dataset contains controlled images (limited real-world variability)
Classification is based on image types, not specific plant diseases
Model performance may vary in real-world environments
# Future Work
Extend classification to actual plant diseases
Use real-world datasets
Deploy on cloud platforms
Improve model interpretability

How to Run the Project (Step-by-Step)
 1. Install Dependencies
pip install -r requirements.txt
 2. Prepare Dataset
Download dataset from Kaggle:
https://www.kaggle.com/datasets/emmarex/plantdisease
Extract it into your project folder:
project/
└── dataset/
 3. Train the Model (Optional)

If you want to train from scratch:

python train.py

 This will:

Load dataset
Train CNN / MobileNetV2
Save model in:
models/best_model_mobilenetv2.pth
 4. Run the Streamlit Application ⭐
streamlit run app.py

 After running, open in browser:

http://localhost:8501
 5. Using the Application
Click “Upload an Image”
Select a plant leaf image
View:
Predicted class
Confidence score
