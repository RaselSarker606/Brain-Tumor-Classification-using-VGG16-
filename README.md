# 🧠 Brain Tumor Classification using VGG16  
**Deep Learning | Medical Imaging | CNN | VGG16 | Transfer Learning**

## 📖 Overview  
This project focuses on classifying brain tumor images using a pre-trained **VGG16** model with transfer learning. It uses deep learning techniques to distinguish between tumor and non-tumor cases (or different tumor types based on the dataset).

---

## 🗂️ Dataset  
The dataset contains brain MRI images categorized into classes:

- Glioma Tumor  
- Meningioma Tumor  
- Pituitary Tumor  
- No Tumor  

*(Update these categories if your dataset is different.)*

---

## 🛠️ Methodology  

### 🔹 Data Preprocessing  
- Resized images to fit VGG16 input (224x224)  
- Applied image augmentation using `ImageDataGenerator`  
- Normalized pixel values (rescaled to [0,1])

### 🔹 Model Architecture  
- Loaded **VGG16** without top layers (pre-trained on ImageNet)  
- Added custom Dense layers for classification  
- Used `Softmax`/`Sigmoid` as output (multi-class or binary)  
- Fine-tuned the top layers for better accuracy

### 🔹 Training  
- Loss Function: `categorical_crossentropy` / `binary_crossentropy`  
- Optimizer: `Adam`  
- Evaluation: Accuracy, Precision, Recall, F1-Score

### 🔹 Visualization  
- Training vs. Validation Accuracy and Loss  
- Confusion Matrix  
- Classification Report

---

## 📊 Results  
- High classification accuracy achieved using **VGG16**  
- The model generalizes well on unseen MRI scans  
- Effective at detecting brain tumors in MRI images

---

brain-tumor-classification-vgg16/
├── Brain_Tumor_classification_VGG16.ipynb
├── dataset/
│   ├── training/
│   ├── validation/
│   └── test/
├── models/
├── README.md
└── requirements.txt

📌 Requirements
Python 3.x
TensorFlow / Keras
NumPy
Matplotlib
scikit-learn
OpenCV (optional)

📎 License
This project is licensed under the MIT License.

## 🚀 How to Run  

1. Clone the repository:
```bash
git clone https://github.com/your-username/brain-tumor-classification-vgg16.git
cd brain-tumor-classification-vgg16
