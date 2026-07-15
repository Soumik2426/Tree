# 🌳 Tree Species Classification using Deep Learning

A comprehensive **Deep Learning-based Tree Species Classification System** that identifies tree species from leaf images using Convolutional Neural Networks (CNNs) and Transfer Learning models.

The project evaluates multiple deep learning architectures, compares their performance using standardized evaluation metrics, and deploys the best-performing model through a **Streamlit** web application.

---

# 📌 Project Highlights

- 🌿 Classifies **30 different tree species**
- 🧠 Trained and evaluated **4 Deep Learning models**
- 📊 Comprehensive model comparison using multiple performance metrics
- 🚀 Streamlit-based web application for real-time prediction
- 📈 End-to-end Deep Learning workflow from preprocessing to deployment

---

# 🚀 Features

- Upload a leaf image and predict its tree species instantly.
- Interactive Streamlit web interface.
- Automatic image preprocessing.
- Multiple trained models available for experimentation.
- Version-controlled model storage.
- Detailed evaluation notebook with comparison graphs and metrics.

---

# 🏗️ Project Workflow

```
Dataset Collection
        │
        ▼
Data Preprocessing
        │
        ▼
Dataset Splitting
(Train / Validation / Test)
        │
        ▼
Model Training

├── Phase 1 : Basic CNN
├── Phase 2 : Improved CNN
├── Phase 3 : EfficientNetB0
└── Phase 4 : MobileNetV2

        │
        ▼
Model Evaluation

├── Accuracy
├── Precision
├── Recall
├── F1 Score
├── Confusion Matrix
├── Classification Report
└── Comparison Graphs

        │
        ▼

Best Model Selection

        │
        ▼

Streamlit Deployment
```

---

# 🗂️ Project Structure

```text
Tree_Species_Classifier/
│
├── app.py                          # Streamlit Web Application
├── requirement.txt                 # Project Dependencies
├── utils/
│   └── model_loader.py             # Model Loading Utilities
│
├── Models/                         # Trained Deep Learning Models (.keras)
│
├── Tree_Species_Dataset/           # Dataset
│
├── Untitled.ipynb                  # Complete Training & Evaluation Notebook
│
└── README.md
```

---

# 📂 Dataset

Dataset contains **1454 leaf images** belonging to **30 tree species**.

### Dataset Split

- Training : **80%**
- Validation : **10%**
- Testing : **10%**

Images are automatically resized to:

```
224 × 224
```

Supported formats:

- JPG
- JPEG
- PNG

---

# 🌿 Tree Species

- Amla
- Asopalav
- Babul
- Bamboo
- Banyan
- Bili
- Cactus
- Champa
- Coconut
- Garmalo
- Gulmohor
- Gunda
- Jamun
- Kanchan
- Kesudo
- Khajur
- Mango
- Motichanoti
- Neem
- Nilgiri
- Other
- Pilikaren
- Pipal
- Saptaparni
- Shirish
- Simlo
- Sitafal
- Sonmahor
- Sugarcane
- Vad

---

# 🤖 Deep Learning Models

The notebook evaluates four different deep learning architectures.

## Phase 1 — Basic CNN

- Baseline Convolutional Neural Network
- Built completely from scratch
- Used as the reference model

---

## Phase 2 — Improved CNN

Enhancements include:

- Additional Convolution Layers
- Global Average Pooling
- Dropout
- Improved architecture
- Better generalization

---

## Phase 3 — EfficientNetB0

Transfer Learning model using ImageNet pretrained weights.

Features:

- EfficientNetB0 Backbone
- Fine-Tuning
- Global Average Pooling
- Regularization
- Learning Rate Scheduling

---

## Phase 4 — MobileNetV2

Final deployment model.

Features:

- ImageNet Pretrained
- Lightweight Architecture
- Fast Inference
- High Accuracy
- Transfer Learning

---

# 📊 Model Performance

| Model | Validation Accuracy | Test Accuracy | Precision | Recall | F1 Score |
|--------|-------------------:|--------------:|----------:|-------:|---------:|
| Basic CNN | 38.24% | 41.43% | 0.3514 | 0.4143 | 0.3514 |
| Improved CNN | 50.00% | 41.43% | 0.3797 | 0.4143 | 0.3608 |
| EfficientNetB0 | 77.94% | 71.43% | 0.7283 | 0.7143 | 0.7084 |
| **MobileNetV2** | **79.41%** | **81.43%** | **0.8556** | **0.8143** | **0.8140** |

---

# 🏆 Best Performing Model

**MobileNetV2**

Performance:

- Validation Accuracy : **79.41%**
- Test Accuracy : **81.43%**
- Precision : **0.8556**
- Recall : **0.8143**
- F1 Score : **0.8140**

MobileNetV2 was selected for deployment because it achieved the highest overall classification performance while remaining computationally efficient.

---

# 📈 Evaluation Metrics

The notebook evaluates every model using:

- Test Accuracy
- Validation Accuracy
- Test Loss
- Precision
- Recall
- F1 Score
- Classification Report
- Confusion Matrix
- Training Curves
- Comparative Analysis

---

# 🧠 Training Pipeline

The notebook follows a standardized TensorFlow `tf.data` pipeline.

Steps include:

- Dataset Loading
- Image Resizing
- Data Augmentation
- Dataset Caching
- Dataset Prefetching
- Model Training
- Model Evaluation
- Model Comparison
- Versioned Model Saving

---

# 💾 Saved Models

All trained models are stored inside:

```
Models/
```

Models are automatically versioned, for example:

```
BasicCNN_v1.keras
ImprovedCNN_v1.keras
EfficientNetB0_v1.keras
MobileNetV2_v1.keras
```

---

# 🖥️ Running the Project

## 1. Clone Repository

```bash
git clone <repository-url>
cd Tree_Species_Classifier
```

---

## 2. Install Dependencies

```bash
pip install -r requirement.txt
```

---

## 3. Launch Streamlit Application

```bash
streamlit run app.py
```

---

## 4. Open Browser

```
http://localhost:8501
```

Upload a leaf image and receive the predicted tree species.

---

# 📦 Requirements

Main libraries used:

- TensorFlow
- Keras
- Streamlit
- NumPy
- Pandas
- Matplotlib
- Scikit-Learn
- Pillow

Install using:

```bash
pip install -r requirement.txt
```

---

# 📚 Notebook Contents

The notebook includes:

- Dataset Preparation
- Data Preprocessing
- Phase 1 – Basic CNN
- Phase 2 – Improved CNN
- Phase 3 – EfficientNetB0
- Phase 4 – MobileNetV2
- Model Evaluation
- Comparative Analysis
- Discussion of Results
- Final Conclusion

---

# 🔮 Future Improvements

Potential enhancements include:

- Larger dataset collection
- Hyperparameter optimization
- More advanced data augmentation
- Vision Transformers (ViT)
- ConvNeXt architecture
- Real-time mobile deployment
- Cloud deployment
- Explainable AI (Grad-CAM)

---

# 📄 License

This project is developed for **educational, research, and learning purposes**.
