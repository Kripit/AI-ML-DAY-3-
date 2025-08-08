# 📌 AI-ML-Day-3 

# 🍕 Food Classification using YOLOv8 (Pretrained)

## 🎯 Goal  
Build a **production-grade** food classification system using **YOLOv8’s classification head**.  

We’ll fine-tune it on the following **5 food classes**:  
- 🍕 Pizza  
- 🍗 Grilled salmon  
- 🍣 Sushi  
- 🍦 Ice Cream  
- 🍔 Hamburger  

## 🚀 Plan  
- Prepare dataset and labels.  
- Use YOLOv8’s classification mode with pretrained weights.  
- Apply **advanced augmentation techniques** to boost performance.  
- Fine-tune and evaluate on validation data.  

## 📊 Output  
A trained model capable of classifying any image into one of the 5 classes above with **high accuracy**.
# AI-ML-DAY-2


This project focuses on building a **production-grade food image classifier** using the **YOLOv8 classification head (`yolov8n-cls.pt`)**, fine-tuned on a subset of the **Food-101 dataset**.

Currently, we are using **5 classes**:
- `pizza`
- `grilled_salmon`
- `sushi`
- `ice_cream`
- `hamburger`

The classifier is designed to be **fast**, **lightweight**, and **highly accurate**, suitable for real-time applications.

--

## 🧠 Model & Dataset

- **Model**: `yolov8n-cls.pt` (YOLOv8 nano)
- **Dataset**: Food-101 (only 5 selected classes used for now)

Folder structure (in progress):


## 📌 Current Status

🟡 **Work in progress**

- [x] Initial config and setup
- [x] Preprocessing + augmentation pipeline
- [x] Dataset structure
- [x] Model training loop (coming soon)
- [x] Evaluation + metrics
- [x] Model saving and inference

📓 Notebook
All code is inside:
Food_Classification_YOLOv8_Module12.ipynb

🚀 what we did 
Implemented the FoodDataset class with Albumentations

Added the training + validation loop

Save and test the fine-tuned model

Maybe test with yolov8s-cls.pt for better accuracy
