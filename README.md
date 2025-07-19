# 🍅 Tomato Plant Disease Detection using InceptionV3 & TensorFlow
This project aims to detect and classify **10 different tomato plant leaf conditions** (including healthy and diseased leaves) using **deep learning**. It leverages **TensorFlow**, **InceptionV3**, and **ImageDataGenerator** to build a high-accuracy image classification model. The goal is to assist farmers and agricultural experts in **early identification of tomato plant diseases**, leading to more effective treatments and improved crop yields.

## ✅ Disease Classes
The model is trained on 10 distinct classes:

1. Tomato\_Bacterial\_spot
2. Tomato\_Early\_blight
3. Tomato\_healthy
4. Tomato\_Late\_blight
5. Tomato\_Leaf\_Mold
6. Tomato\_Septoria\_leaf\_spot
7. Tomato\_Spider\_mites (Two-spotted spider mite)
8. Tomato\_Target\_Spot
9. Tomato\_Yellow\_Leaf\_Curl\_Virus
10. Tomato\_mosaic\_virus

### 🗂️ Dataset

The dataset was sourced from the **PlantVillage** dataset, a well-known public dataset for plant disease detection. Images are labeled by experts and cover a wide variety of disease symptoms under different lighting and angle conditions.
#### I am attaching the kaggle site for the dataset: "https://www.kaggle.com/datasets/noulam/tomato".

### 🧠 Model Architecture

* **Base Model**: InceptionV3 (pretrained on ImageNet, with `include_top=False`)
  
* **Top Layers**:
  * Global Average Pooling
  * Dense (1024 units, ReLU)
  * Dense (10 units, Softmax)
    
* **Framework**: TensorFlow + Keras
  
* **Image Preprocessing**: ImageDataGenerator with data augmentation
  
* **Training Input Size**: 224x224

### 📊 Results
The model achieved **high accuracy** in classifying tomato leaf diseases, with performance validated on a held-out validation set.

#### Evaluation Metrics:
* Accuracy
* Loss
* Confusion Matrix (Recommended)
* Classification Report

### 🌱 Applications
* Early disease detection for farmers and agronomists
* Integration into a mobile/web app for real-time leaf diagnosis
* Educational tool for learning plant pathology with AI


