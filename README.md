# CoffeeBean Quality Classification - Mobile Application and ML Models

This repository contains the complete framework developed for the project **"Deep Learning-Powered Mobile Application for Coffee Bean Quality Classification"**, including:

* 📱 A **Flutter-based Mobile Application** for real-time coffee bean quality classification.
* 🧠 **Machine Learning models** trained for 5-class classification of Arabica coffee beans.
* 📊 A **publicly available coffee bean image dataset**.
* 🖥️ Optional **Python-based API backend** for remote inference and logging.

---

## 🏆 Project Overview

Manual coffee bean classification is subjective, time-consuming, and prone to error. This project introduces an automated solution using deep learning and computer vision techniques for classifying **five quality categories of Arabica coffee beans**, namely:

1. Soft (Mole)
2. Hard (Duro)
3. Slightly Fermented (Riado)
4. Fermented (Rio)
5. Highly Fermented (Rio Zona)

The best-performing model (**YOLOv11-nano-cls**) was integrated into a **cross-platform mobile application** (Flutter + TFLite) that works **offline and in real-time**, making it suitable for use by coffee producers directly on the field.

---

## 📂 Repository Structure

```
.
├── dataset/               # Link to Roboflow workspace with coffee bean image dataset
├── models/                # Trained models (YOLOv11, MobileNetV2, MobileViT, etc.)
├── notebooks/             # Google Colab and Jupyter notebooks for training and evaluation
└── README.md              # This file
```

---

## 🧬 Dataset

* 📸 **Total Images:** 511 original, expanded to 1,209 with augmentation.
* 🏞️ **Image Resolution:** 256x256 pixels.
* 📋 **Classes:** Soft, Hard, Slightly Fermented, Fermented, Highly Fermented.

---

## 🧠 Machine Learning Models

### Models Tested:

* ConvMixer
* FNet
* gMLP
* MLP-Mixer
* MobileNetV2
* MobileViT
* Vision Transformer (ViT)
* YOLOv11-nano-cls ✅ **(Best Model)**
* YOLOv11-small-cls
* YOLOv11-medium-cls

### Best Results:

| Model                      | Accuracy | F1-Score  |
| -------------------------- | -------- | --------- |
| YOLOv11-nano + Mode Voting | **97%**  | **97.1%** |

📌 Full training and evaluation details are available in the `notebooks/` folder.

---

## 📱 Mobile Application (Flutter + TFLite)

Features:

* Offline inference on Android and iOS.
* Automatic capture of 3 sequential images.
* Majority voting (mode calculation) for improved accuracy.
* Intuitive and minimal UI.

> Note: The app uses **TensorFlow Lite (TFLite)** for on-device inference.

➡️ **[Mobile Application Download](https://github.com/zz4fap/CoffeeClassificator-API)**

---

## 📈 Results Summary

* ✅ Over **90% accuracy** on mobile testing with real samples.
* ✅ Inference time suitable for real-time field use (\~1.2s per image on smartphone).
* ✅ Supports **offline classification** without internet access.

---

## 🗺️ Roadmap / Future Work

* Expand dataset with more samples and classes.
* Integrate aroma and flavor detection (electronic nose/tongue).
* Optimize for TinyML (e.g., Edge Impulse, MCUs).
* Add user data logging and cloud-based analytics dashboard.

---

## 👩‍💻 Contributors

* **Isabela V. de Carvalho Motta**
* **Felipe A. P. de Figueiredo**
* **Henrique R. Mendonça**
* **Samuel B. Mafra**
* **Jayme G. A. Barbedo**

---

## 📄 License

This project is licensed under the GNU General Public License v3.0 (GPL-3.0).

➡️ See full license text here: https://www.gnu.org/licenses/gpl-3.0.html

---

## 📚 Citation

If you use this project or dataset in your research, please cite:

```
@article{Motta2025,
  title={Deep Learning-Powered Mobile Application for Coffee Bean Quality Classification},
  author={Isabela V. de Carvalho Motta, Felipe A. P. de Figueiredo, Henrique R. Mendonça, Samuel B. Mafra, Jayme G. A. Barbedo},
  journal={Arxiv},
  year={2025}
}
```

---
