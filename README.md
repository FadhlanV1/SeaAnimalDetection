# 🐠 Sea Animals Classification using MobileNetV2

Proyek ini bertujuan untuk membangun model klasifikasi gambar hewan laut dengan pendekatan *Transfer Learning* menggunakan arsitektur **MobileNetV2**. Proyek ini sangat cocok untuk pembelajaran *computer vision*, riset ekologi laut, dan pengembangan aplikasi edukatif mengenai kehidupan bawah laut.

---

## 📂 Dataset

- **Nama Dataset:** Sea Animals Domain Adaptation Dataset  
- **Sumber:** [Kaggle Dataset](https://www.kaggle.com/datasets/gusanagy/sea-animals-domain-adaptation-dataset)
- **Jumlah Kelas:** 9 jenis hewan laut  
- **Struktur Dataset:** Setiap folder merepresentasikan satu kelas hewan laut dan berisi gambar-gambar terkait, memudahkan proses pelatihan menggunakan TensorFlow atau PyTorch.

---

## 🧠 Arsitektur Model

Model dikembangkan dengan pendekatan *Transfer Learning* menggunakan:

- **Base model:** MobileNetV2 (pre-trained on ImageNet)
- **Preprocessing:** Image cropping, resizing (224×224), normalisasi
- **Layers tambahan:**
  - `GlobalAveragePooling2D`
  - `Dense(ReLU)`
  - `Dropout`
  - `Dense(Softmax)` untuk output 9 kelas

Model dikompilasi menggunakan:

- **Optimizer:** Adam  
- **Loss Function:** Categorical Crossentropy  
- **Metrics:** Accuracy

---

## ⚙️ Tools & Framework

- Python
- Google Colab / Jupyter Notebook
- TensorFlow & Keras
- Matplotlib
- splitfolders
- zipfile, os, shutil

---
