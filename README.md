# Business Problem:
## Background
Source: 
Pneumonia is an inflammatory condition of the lung affecting primarily the small air sacs known as alveoli.Symptoms typically include some combination of productive or dry cough, chest pain, fever and difficulty breathing. The severity of the condition is variable. Pneumonia is usually caused by infection with viruses or bacteria and less commonly by other microorganisms, certain medications or conditions such as autoimmune diseases.Risk factors include cystic fibrosis, chronic obstructive pulmonary disease (COPD), asthma, diabetes, heart failure, a history of smoking, a poor ability to cough such as following a stroke and a weak immune system. Diagnosis is often based on symptoms and physical examination. Chest X-ray, blood tests, and culture of the sputum may help confirm the diagnosis.The disease may be classified by where it was acquired, such as community- or hospital-acquired or healthcare-associated pneumonia.

Source: https://www.hopkinsmedicine.org/health/conditions-and-diseases/pneumonia
## Problem Statement
We need to be able to quickly and accurately identify which patients have pneumonia using a model, so that doctors themselves spend less time reviewing images.
# This project was created using the following libraries:
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import keras
from keras.models import Sequential
from keras.layers import Dense, Conv2D , MaxPool2D , Flatten , Dropout , BatchNormalization
from keras.preprocessing.image import ImageDataGenerator, load_img
from sklearn.model_selection import train_test_split
from sklearn.metrics import classification_report,confusion_matrix
from keras.callbacks import ReduceLROnPlateau
import cv2
import os
from PIL import Image

## Repository Structure

```
├── .ipynb_checkpoints
├── Data
├── Images
├── README.md
├── x-ray-image-analysis-Jupyter_Notebook.pdf
├── x-ray-image-analysis.ipynb
├── X-ray-analysis.pdf
└── github.pdf
