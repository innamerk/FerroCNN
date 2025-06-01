# FerroCNN
CNN-MagneticParameterPrediction


---

# Predicting Magnetic Anisotropy of Magnetoactive Elastomers from Microstructure Images

### 👩‍🔬 Authors

Inna I. Merkoulova, Viktor A. Nemchenko, Dmitry I. Merkoulov, Daria A. Pelevina

---

### 🧠 Description

This project explores the use of a convolutional neural network (**EfficientNet-B0**) to predict the **magnetic anisotropy parameter** of anisotropic magnetoactive elastomers (AMEs) from microscope images of ferro-particle microstructures.

The model is fine-tuned on a custom dataset and evaluated on previously unseen configurations. Grad-CAM is used to interpret the regions of the image most relevant to the prediction.

---

### 📁 Project Structure

```
FerroCNN/
├── data/                        # Example images from the dataset
│   └── *.jpg
│   └── target.xlsx
├── notebooks/
│   └── IIM_FERRO_CNN.ipynb     # Jupyter Notebook with full pipeline
├── examples/                   # Grad-CAM visualization results
│   └── gradcam_*.png
├── LICENSE                     # Custom restrictive license
└── README.md
```

---

### 🚀 Quick Start

1. Clone the repository:

```bash
git clone https://github.com/innamerk/FerroCNN.git
cd FerroCNN
```

2. Open the main notebook for training and testing:

```bash
jupyter notebook notebooks/IIM_FERRO_CNN.ipynb
```

> **Note:** All dependencies are listed and installed directly within the notebook.

3. Download the trained model weights:

[📥 Download EfficientNet-B0 weights](https://drive.google.com/file/d/1b7SEAk3zkkBlTRztkKxI_8Eo52QAcQeF/view?usp=sharing)

---

### 📊 Results

| Metric | Test Set | New Unseen Set |
| -----: | -------: | -------------: |
|    MAE |     0.09 |         \~0.12 |
|    MSE |     0.02 |         \~0.02 |

Grad-CAM heatmaps (see `examples/`) confirm the model attends to physically meaningful features like particle chains and structural alignment patterns.

---

### 📰 Reference

> **Determining Magnetic Parameters of Anisotropic Magnetoactive Elastomers Based on Microstructure Images**
> *Merkoulova I.I., Nemchenko V.A., Merkoulov D.I., Pelevina D.A.*

---

### ⚠️ License

This repository is protected by a **custom restrictive license**.

> *Any use, reproduction, distribution, or modification is strictly prohibited without explicit permission from the authors.*

---



