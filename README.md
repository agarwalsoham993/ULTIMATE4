# Skin Cancer Prediction Model

Overview
This repository houses a skin cancer prediction model trained on a massive dataset of over 4,00,000 entries and their corresponding high-resolution images. The primary goal of this project is to develop a highly accurate and robust deep learning model to assist in the early detection and classification of various types of skin lesions, thereby supporting medical professionals in their diagnostic process.

Dataset
The model was trained on a comprehensive dataset comprising approximately 400,000 images of skin lesions. Each entry includes:

Images dataset :- Individual image corresponding to the ISIC_ID
Metadata:- https://docs.google.com/document/d/1Jk9W9s0RRX3H42afKa6vDhy7ejoaPH0l-M-atpV0zL0/edit?usp=sharing

The dataset has been meticulously cleaned, preprocessed, and augmented to ensure high quality and to mitigate potential biases.


Model Architecture :
This project utilizes a state-of-the-art deep learning architecture, leveraging a [mention specific architecture, e.g., Convolutional Neural Network (CNN)] for image feature extraction and classification. The model's design is optimized for performance, scalability, and interpretability.

## Image - Pre-Processing

The images dataset consists of snapshots of skin samples, of varying resolutions. The pre-processing step mainly consists of standardising the images and extracting lesions (if present) from them. This ensures that the Convolutional Neural Network is able to extract maximum information from the data.
Our approach consisted of Cleaning and Normalizing the iamges followed by feature extraction.

Cleaning and Normalizing:
1. Resizing: Resized all images to a resolution of (224,224)

2. Normalizing the images

Feature Extraction:
1. CLAHE: Histogram Equalization is applied on the images. This process enhances contrast in images, which is a key step in increasing brightness and visibility in certain regions.
   
2. Lesion Extraction: Using a series of thresholding and morphological operations (opening and dilation) to isolate the lesion area and then uses this as a mask to blacken the rest of the image.
   

## Base Model: 

Layers: A series of convolutional layers, pooling layers, and fully connected layers.

Activation Functions: 

Loss Function:

Optimizer: 

## Performance
The model's performance on the validation and test sets is as follows:

Accuracy: 

Precision:

Recall:

F1-Score:

## Getting Started
Prerequisites :-

  Python [mention version, e.g., 3.8+]
  
Libraries used :-

  Numpy,Pandas,Matplotlib,seaborn


## Team (Contributors) :

Soham agarwal (https://github.com/agarwalsoham993/)

Keshab Agarwal (https://github.com/karl-1-bit/)

Sounika Mandal (https://github.com/Megha06-byte/)

Mangalam sharma (https://github.com/PrincipledProgrammer/)

Ayush Kuril

Nikhil Arimakala

Shaurya Shreyas

Shatakshi Shukla

Shaurya Pratap
