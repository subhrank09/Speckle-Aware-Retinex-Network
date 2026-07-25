# 🌌 SARD-Net: Speckle-Aware Retinex Decomposition Network for Low-Light SAR Image Restoration

> A deep learning framework for enhancing low-light Synthetic Aperture Radar (SAR) images while preserving structural details using Retinex decomposition and speckle-aware optimization.

![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-DeepLearning-red)
![OpenCV](https://img.shields.io/badge/OpenCV-ComputerVision-green)

---

## 📌 Overview

Synthetic Aperture Radar (SAR) imagery is widely used for remote sensing because it can operate under all-weather and day/night conditions. However, SAR images captured under low-light conditions often suffer from:

- Speckle Noise
- Poor Illumination
- Loss of Structural Information
- Low Visual Quality

This project proposes a **Speckle-Aware Retinex Decomposition Network (SARD-Net)** that restores low-light SAR images while preserving fine structural details.

---

## ✨ Features

- Speckle-aware Retinex decomposition
- Improved U-Net architecture
- Encoder–Decoder with skip connections
- Custom SSIM Loss
- Speckle Loss
- Combined Loss Function
- Mixed Precision Training (AMP)
- Automatic Checkpoint Saving
- Learning Rate Scheduling
- Baseline U-Net Comparison
- Ablation Study
- PSNR & SSIM Evaluation

---

# 🏗 Architecture

```
Low-Light SAR Image
        │
        ▼
Retinex Decomposition
        │
        ▼
Feature Encoder
        │
        ▼
Improved U-Net
        │
        ▼
Feature Decoder
        │
        ▼
Enhanced SAR Image
```

---

# 📂 Dataset

The model is trained on paired SAR-Optical images separated by terrain classes.

Dataset Categories:

- Agriculture
- Grassland
- Urban
- Barren Land

Dataset Split

| Split | Images |
|--------|--------|
| Train | 12,800 |
| Validation | 1,600 |
| Test | 1,600 |

---

# 🧠 Model Components

## Retinex Decomposition

Separates:

- Illumination
- Reflectance

to improve image restoration.

---

## Improved U-Net

The network consists of:

- Double Convolution Blocks
- Encoder
- Decoder
- Skip Connections
- Residual Learning

---

## Custom Loss Function

The final loss combines

- L1 Loss
- SSIM Loss
- Speckle Loss

to simultaneously improve:

- Image Quality
- Structural Preservation
- Noise Suppression

---

# 📊 Evaluation Metrics

Model performance is evaluated using

- PSNR
- SSIM
- Validation Loss
- Test Loss

---

# 🔬 Experiments

The notebook includes:

- Model Training
- Validation
- Testing
- Checkpoint Loading
- Baseline Comparison
- Ablation Study

---

# 🛠 Tech Stack

- Python
- PyTorch
- NumPy
- OpenCV
- Matplotlib
- Pandas
- Scikit-image
- Scikit-learn

---

# 📁 Repository Structure

```
├── sar-research-work.ipynb
├── README.md
```

---

# 🚀 Running

Clone the repository

```bash
git clone https://github.com/yourusername/SARD-Net-Low-Light-SAR-Image-Restoration.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run

```bash
jupyter notebook
```

Open

```
sar-research-work.ipynb
```

---

# 📈 Future Improvements

- Transformer-based image restoration
- Attention-guided Retinex decomposition
- Real-time inference optimization
- Lightweight deployment model
- ONNX / TensorRT export
- Multi-GPU distributed training

---

# 👨‍💻 Author

**Subhrank Priya**

B.Tech Computer Science Engineering

Machine Learning Engineer | AI Researcher | Computer Vision Enthusiast

GitHub: https://github.com/subhrank09

Portfolio: https://subhrank-priya.vercel.app

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.
