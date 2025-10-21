# 🩺 Deep Learning for Retinal OCT Disease Classification

## 📘 Overview
This project is a **team-based research initiative** that leverages **deep learning** to classify retinal diseases using **Optical Coherence Tomography (OCT)** images.  
Our objective is to enable **early, reliable, and automated detection** of major retinal disorders — helping ophthalmologists diagnose eye diseases faster and more accurately.

The project integrates **multiple CNN architectures** through an **ensemble learning framework** to improve overall diagnostic performance and reduce false predictions.

---

## 🧩 Key Features
- 🧠 **Ensemble CNN Models:** Combines ResNet, VGG, and Inception for improved accuracy.  
- 🧺 **Data Pipeline:** Automated preprocessing, augmentation, and stratified data splitting.  
- ⚙️ **Training Framework:** Includes adaptive learning rate scheduling and early stopping.  
- 📊 **Evaluation Suite:** Confusion matrix, accuracy, F1-score, and class-specific metrics.  
- 💾 **Model Persistence:** Saves best-performing weights automatically for deployment.  
- 🌐 **Future Ready:** Designed for integration with Flask/Streamlit apps.

---

## 📂 Dataset
We used the **Retinal OCT Images (Kermany et al.)** dataset, publicly available on [Kaggle](https://www.kaggle.com/paultimothymooney/kermany2018).  
It consists of the following four classes:

| Class | Description |
|:------|:-------------|
| **CNV** | Choroidal Neovascularization |
| **DME** | Diabetic Macular Edema |
| **DRUSEN** | Drusen deposits |
| **NORMAL** | Healthy retina images |

---

## ⚙️ Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/your-org/retinal-oct-diagnosis.git
cd retinal-oct-diagnosis
```
Run the first cell in the jupyter notebook file for the installation of requirements

---

## 🚀 Usage
Run the notebook to train and evaluate the model:
```bash
jupyter notebook retinal_oct_train.ipynb
```
Or execute the training script directly (if converted to `.py`):
```bash
python retinal_oct_train.py
```

---

## 🧪 Model Evaluation
Example performance results:

| Metric | Value |
|:-------|------:|
| Accuracy | 98.4% |
| Precision | 97.9% |
| Recall | 98.2% |
| F1-score | 98.0% |

---

## 🧠 Ensemble Strategy
The ensemble learning module combines multiple CNN predictions:
```python
final_pred = (resnet_pred + vgg_pred + inception_pred) / 3
```
This boosts reliability by leveraging the strengths of individual architectures.

---

## 👨‍💻 Team Members
| Name | Role | Responsibilities |
|:------|:------|:----------------|
| **Dheeraj Chandra** | Team Lead / Developer | Project design, model implementation, documentation |
| **Sumith Chandra** | Research & Dataset Engineer | Data preprocessing, augmentation, analysis |
| **Venkat Reddy** | Model Engineer | CNN architecture design, ensemble tuning |
| **Vijay Chandra** | Evaluation & Deployment | Metrics evaluation, deployment setup |

---

## 🏫 Institution
**Department of Computer Science and Engineering**  
**B.Tech Program, 3rd Year**  
**Gokaraju Rangaraju Institute Of Engineering And Technology**  

---

## ✨ Acknowledgements
We thank our faculty mentors and peers for their guidance and support in realizing this project.  

> *"AI doesn’t replace doctors — it empowers them to see more clearly."* 🧠



