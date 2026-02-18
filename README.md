# Smart-Sorting-Transfer-Learning-for-Identifying-Rotten-Fruits-and-Vegetables
Smart Sorting Transfer Learning for Identifying Rotten Fruits and Vegetables
## 🔍 Overview
**Smart Sorting** is a deep learning-based web application that classifies images of fruits and vegetables as **fresh or rotten** using **transfer learning with EfficientNetB0**. It aims to reduce food waste and assist in **automated quality control** for supermarkets, smart kitchens, and food processing industries.

## 🎯 Objective
To build a lightweight, intelligent, and real-time fruit & vegetable freshness detection system that:
- Minimizes food spoilage and manual errors.
- Provides a deployable web interface for predictions.
- Helps in smart home and retail automation.

---

## 🧠 Model Highlights

| Feature              | Description                                 |
|----------------------|---------------------------------------------|
| Base Model           | EfficientNetB0 (ImageNet pretrained)        |
| Input Image Size     | 224x224                                     |
| Training Enhancements| MixUp Augmentation, Cosine Decay LR, Dropout |
| Fine-Tuning          | Last 50 layers of base model                |
| Exported Format      | `.keras`                                    |

---

## 🗂️ Dataset
- **Source**: [Kaggle - Fruits Fresh and Rotten for Classification](https://www.kaggle.com/datasets/kritikseth/fruit-and-vegetable-image-recognition)
- **Classes**: 206 (Fresh/Rotten fruits & vegetables)
- **Images**: ~104,000
- **Resized To**: 224×224 for training
- **Saved File**: `class_indices.json`

---

## ⚙️ Tech Stack

| Component     | Version       | Purpose                  |
|---------------|---------------|--------------------------|
| Python        | 3.9+          | Backend + Training       |
| TensorFlow    | 2.11+         | Model & Training         |
| Flask         | 2.0+          | Web API & Deployment     |
| HTML/CSS/JS   | -             | Frontend Interface       |
| Anaconda      | Any           | Environment Management   |
| tfp, Pillow   | Latest        | Augmentation/Image I/O   |

---

## 📁 Project Structure
Smart_Sorting/
│
├── app.py # Flask backend
├── train_model.py # Model training pipeline
├── config.py # Configuration variables
├── templates/
│ └── index.html # Frontend HTML
├── static/
│ ├── style.css # Frontend styles
│ └── script.js # JS interaction logic
├── models/
│ ├── fruit_classifier_effnet_light.keras
│ └── class_indices.json
└── README.md # Project documentation

## 🚀 Features

- 🔎 Real-time image classification with confidence score.
- 🔄 Advanced training pipeline using MixUp, cosine decay, and label smoothing.
- 🧠 Model trained on 206 classes with >99% validation accuracy.
- 🖼️ Intuitive UI for image upload and prediction.
- 🌐 Flask API with `/predict` and `/health` endpoints.
- ✅ Displays predictions **only if confidence > 55%**.


Visit: http://127.0.0.1:5000


🎯 Use Cases
🛒 Supermarkets: Auto-detection of spoilage on shelves.

🚜 Farmers: Post-harvest quality control.

🏠 Smart Homes: Smart kitchen freshness detection.

🧪 Food Tech Startups: Integrate into IoT & SaaS QC platforms.

🏁 Final Output
✅ Model trained with 99%+ accuracy

✅ Real-time web app predictions

✅ Confidence thresholding at 55%

✅ UI ready for deployment

🙌 Credits
EfficientNet by Google AI

Dataset by Kritik Seth on Kaggle
📬 Contact
Koppineedi Lakshmi Prasanna
📧 prasannakoppineedi@gmail.com
🌐 LinkedIn: https://www.linkedin.com/in/prasanna-koppineedi-249825316/
📂 GitHub:(https://github.com/prasannaKoppineedi01)
