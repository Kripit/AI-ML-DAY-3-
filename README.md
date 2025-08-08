🍕 Food Classification using YOLOv8 (Pretrained)
This project builds a production-grade food image classifier using the YOLOv8 classification head (yolov8n-cls.pt), fine-tuned on a subset of the Food-101 dataset.

We’ve started with 5 delicious classes:

🍕 pizza

🐟 grilled_salmon

🍣 sushi

🍦 ice_cream

🍔 hamburger

The goal? Fast, lightweight, highly accurate — ready for real-time applications.

✅ Features
YOLOv8 Classification Head — pretrained on ImageNet

Albumentations for advanced image augmentation

Cosine Annealing LR Scheduler for smoother training convergence

Custom Config class for clean project settings

Structured logging system to track training and errors

Support for YOLOv8 Nano (fastest) and YOLOv8 Small (better accuracy)

Ensemble predictions combining both models

🧠 Model & Dataset
Model:

Base: yolov8n-cls.pt (Nano) & yolov8s-cls.pt (Small)

Fine-tuned for our 5-class food subset

Dataset:

Food-101 — only selected 5 classes

Balanced train/test split

Max images per class: 100 (train)

Test images per class: 20

Folder Structure:

markdown
Copy
Edit
food-101/
  images/
    pizza/
    grilled_salmon/
    sushi/
    ice_cream/
    hamburger/
📌 Current Status
🟡 Work in Progress
✔ Initial config & setup
✔ Preprocessing + augmentation pipeline
✔ Dataset loader with Albumentations
⬜ Model training loop (almost done)
⬜ Evaluation + metrics
⬜ Model saving & inference scripts

🚀 Today's Progress (Day 3)
Implemented FoodDataset class with Albumentations

Added training + validation loops

Enabled saving & testing the fine-tuned model

Added optional YOLOv8 Small model for better accuracy tests

⚡ Quick Start
1️⃣ Clone the repo & install dependencies

bash
Copy
Edit
git clone https://github.com/yourusername/Food-Classification-YOLOv8.git
cd Food-Classification-YOLOv8
pip install -r requirements.txt
2️⃣ Download Food-101 dataset
Place the images under:

bash
Copy
Edit
./foof/food-101/images/<class_name>/
3️⃣ Run training

bash
Copy
Edit
python train.py
4️⃣ Test inference

bash
Copy
Edit
python classify.py --image path/to/image.jpg
📊 Training Pipeline
Augmentations Used:

Resize → Horizontal Flip → Rotation (±15°)

Brightness/Contrast tweak

Gaussian Noise

Motion Blur

ImageNet normalization

Training Highlights:

Batch size optimized for GPU

Cosine Annealing LR

Ensemble predictions for higher confidence

🔮 Next Steps
 Hyperparameter tuning

 Experiment with larger YOLO models for accuracy boost

 Deploy API endpoint for real-time classification

 Integrate with a mobile app for camera-based inference

