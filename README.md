# 🧬 Cervical Cancer Detection using Hybrid Deep Learning Models

Cervical cancer is one of the most preventable and treatable forms of cancer when detected early. However, delays in screening and diagnosis—especially in under-resourced regions—can lead to late-stage discoveries, reduced treatment success, and ultimately, loss of life.

This project leverages **deep learning and hybrid feature extraction** techniques to automate and enhance the accuracy of cervical cell classification from microscopic images, potentially assisting pathologists in early diagnosis.

---

## 🚀 Highlights

- 📂 **Multi-class classification** of 5 types of cervical cells
- 🔍 **Hybrid model** combining ResNet50, DenseNet121, and EfficientNetB5 for deep feature extraction
- ⚙️ **Dimensionality reduction** using PCA
- 🧠 **Feed-forward Neural Network** for final classification
- 📊 Precision, Recall, F1-Score, Confusion Matrix, and ROC Curve analysis

---

## 🧠 Problem Statement

The manual analysis of cervical cytology slides is time-consuming, prone to human error, and often inconsistent. The objective is to **develop an AI-powered, reliable model** to classify cervical cell types from Pap smear images and assist medical professionals in making timely and accurate diagnoses.

---

## 📂 Dataset Description

The dataset consists of 5 labeled categories of cervical cells:

1. Dyskeratotic  
2. Koilocytotic  
3. Metaplastic  
4. Parabasal  
5. Superficial-Intermediate

Each class folder contains **CROPPED** microscopic images of cells captured during Pap smear tests.

---

## ⚙️ ML/DL Models Used

### 🧬 Feature Extractors:
- **ResNet50**
- **DenseNet121**
- **EfficientNetB5**

These models were used *without the top classification layer* to extract deep features from images.

### 🧠 Classifier:
- Features from all three CNNs were **concatenated**, normalized using **MinMaxScaler**, and **reduced with PCA**.
- A **simple Dense Neural Network** was trained on these reduced features for final prediction.

---

## 📊 Evaluation Metrics

- ✔️ Accuracy: **High classification accuracy** achieved on test data
- 📈 ROC AUC (Micro-average): `>0.95`
- 📉 Confusion Matrix: Visualizes true vs predicted labels
- 📊 Class-wise comparison of Precision, Recall, and F1 Score

All models and evaluation plots are available in the notebook.

---

## 🌍 Real-World Impact

- 🏥 Could significantly assist **cytopathologists** in decision-making
- 💡 Reduces **workload and diagnostic error**
- 🧪 Promotes early **screening in rural/underserved areas** using portable AI solutions

---

## 📎 How to Use

1. Clone the repo or open the notebook in [Google Colab](https://colab.research.google.com/)
2. Upload the dataset (linked in the notebook)
3. Run all cells to extract features, train the model, and evaluate performance

---

## 🖼️ Visualizations

- 📊 Bar plots for precision, recall, and F1 score per class
- 📉 Confusion matrix with class annotations
- 🔍 ROC Curve for each class
- 🥧 Pie chart of class distribution

---

## 🤝 Credits

Project developed by **Prasanna Devireddy**  
- 🔗 [LinkedIn](https://www.linkedin.com/in/prasanna-devireddy/)  
- 💻 [GitHub](https://github.com/PrasDev4)  
- 📫 prasannadevireddy4@gmail.com

---

## 📜 License

This project is for educational and research purposes only. Please cite appropriately if used.
