# 🩺 Deep Learning for Retinal OCT Disease Classification

## 📘 Overview
This project presents a **deep learning-based diagnostic system** for classifying retinal diseases using **Optical Coherence Tomography (OCT)** images. The notebook `retinal_oct_train.ipynb` implements a full pipeline — from data preprocessing to model evaluation — leveraging convolutional neural networks (CNNs) for automated eye disease detection.

The primary goal is **early and accurate detection of retinal disorders** such as *Choroidal Neovascularization (CNV)*, *Diabetic Macular Edema (DME)*, *Drusen*, and *Normal* eyes.

---

## 🧩 Key Features
- ✅ **Data Preprocessing:** Efficient loading, normalization, and augmentation of OCT images.  
- 🧠 **Model Architectures:** Ensemble of CNN models (e.g., ResNet, VGG, Inception).  
- ⚙️ **Training Pipeline:** Customizable training with learning rate scheduling and early stopping.  
- 📈 **Evaluation:** Classification metrics (Accuracy, F1-score, Confusion Matrix).  
- 💾 **Model Saving:** Automatically stores best-performing weights for reuse or deployment.  

---

## 📂 Dataset
The dataset used is the **Retinal OCT Images (Kermany et al.)**, publicly available on [Kaggle](https://www.kaggle.com/paultimothymooney/kermany2018).  
It contains four categories:
- `CNV` – Choroidal Neovascularization  
- `DME` – Diabetic Macular Edema  
- `DRUSEN` – Drusen deposits  
- `NORMAL` – Healthy retina images  

---

## ⚙️ Installation
Clone this repository and install dependencies:
```bash
git clone https://github.com/your-username/retinal-oct-diagnosis.git
cd retinal-oct-diagnosis
pip install -r requirements.txt
```

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
Typical metrics observed (example values):
| Metric | Value |
|:-------|------:|
| Accuracy | 98.4% |
| Precision | 97.9% |
| Recall | 98.2% |
| F1-score | 98.0% |

---

## 🧠 Ensemble Strategy
This project optionally supports **ensemble learning**, combining predictions from multiple CNN models to enhance robustness and generalization.

Ensemble example:
```python
final_pred = (resnet_pred + vgg_pred + inception_pred) / 3
```

---

## 💡 Future Work
- Incorporate **Vision Transformers (ViT)** for performance comparison.  
- Develop a **Flask/Streamlit web interface** for interactive diagnosis.  
- Integrate **Grad-CAM** for explainability visualization.  

---

## 🩸 Citation
If you use this work, please cite:
```
@article{retinaloct2025,
  title={Deep Learning and OCT Imaging: A Novel Ensemble Approach for Eye Disease Diagnosis},
  author={V Vijay Chandra},
  year={2025},
  journal={Independent Research Project}
}
```

---

## 👤 Author
**Vijay Chandra Vinnakota**  
B.Tech, 3rd Year | AI & ML Enthusiast  
GitHub: [@your-username](https://github.com/Vijay-Chandra-11)

---
> *“Early detection saves vision — empowering AI to see what humans can’t.”*
