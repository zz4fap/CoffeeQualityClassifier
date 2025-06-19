# Coffee Bean Quality Dataset

This folder contains the **Coffee Bean Quality Classification Dataset** used in the project *"Deep Learning-Powered Mobile Application for Coffee Bean Quality Classification"*.

The dataset was designed to support the classification of Arabica coffee beans into **five quality categories**:

* Soft (Mole)
* Hard (Duro)
* Slightly Fermented (Riado)
* Fermented (Rio)
* Highly Fermented (Rio Zona)

---

## 📅 Dataset Versions Summary

Throughout the research and model development phases, **30 dataset versions** were created. These versions differ in **image resolution**, **preprocessing steps**, **data augmentation techniques**, and **training-validation-test split strategies**.

The table below summarizes the key characteristics of each dataset version:

---

## 📊 Dataset Evolution

| Version | Total Images | Dataset Split                                     | Preprocessing                                                                                   | Augmentations                                                                                                                                                                 |
| ------- | ------------ | ------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 01      | 195          | Train Set: 180<br>Test Set: 15                    | Auto-Orient: Applied<br>Resize: Stretch to 640x640                                              | Outputs per training example: 3<br>Flip: Horizontal<br>Crop: 0% Min Zoom, 20% Max Zoom<br>Shear: ±10° Horizontal/Vertical                                                     |
| 02      | 195          | Train Set: 180<br>Test Set: 15                    | Auto-Orient: Applied<br>Resize: Stretch to 640x640                                              | Outputs per training example: 3<br>Flip: Horizontal, Vertical<br>Crop: 0%-50% Zoom<br>Shear: ±25°<br>Brightness: -15% to +15%<br>Blur: Up to 1px<br>Noise: Up to 1.49% pixels |
| 03      | 753          | Train Set: 753                                    | Auto-Orient: Applied<br>Resize: Stretch to 640x640                                              | Outputs per training example: 3<br>Flip: Horizontal<br>Crop: 0%-20% Zoom<br>Shear: ±10°                                                                                       |
| 04      | 873          | Train Set: 858<br>Valid Set: 10<br>Test Set: 5    | Auto-Orient: Applied<br>Resize: Stretch to 160x160                                              | Outputs per training example: 3<br>Flip: Horizontal, Vertical<br>Crop: 0%-50% Zoom<br>Shear: ±25°<br>Brightness: -15% to +15%<br>Blur: Up to 1px<br>Noise: Up to 1.49% pixels |
| 05      | 783          | Train Set: 723<br>Valid Set: 60                   | Auto-Orient: Applied<br>Resize: Stretch to 160x160                                              | Outputs per training example: 3<br>Flip: Horizontal, Vertical<br>Crop: 0%-15% Zoom<br>Shear: ±15°<br>Brightness: -15% to +15%<br>Blur: Up to 1px<br>Noise: Up to 1.49% pixels |
| 06      | 783          | Train Set: 723<br>Valid Set: 55<br>Test Set: 5    | Same as Version 05                                                                              | Same as Version 05                                                                                                                                                            |
| 07      | 783          | Train Set: 723<br>Valid Set: 30<br>Test Set: 30   | Same as Version 05                                                                              | Same as Version 05                                                                                                                                                            |
| 08      | 301          | Train Set: 301                                    | Auto-Orient: Applied<br>Resize: Stretch to 32x32                                                | No augmentations                                                                                                                                                              |
| 09      | 301          | Train Set: 241<br>Valid Set: 30<br>Test Set: 30   | Same as Version 08                                                                              | No augmentations                                                                                                                                                              |
| 10      | 783          | Train Set: 723<br>Valid Set: 30<br>Test Set: 30   | Auto-Orient: Applied<br>Resize: Fill (center crop) 640x640                                      | Outputs per training example: 3<br>Flip: Horizontal, Vertical<br>90° Rotate CW/CCW<br>Rotation: ±15°                                                                          |
| 11      | 782          | Train Set: 722<br>Valid Set: 30<br>Test Set: 30   | Auto-Orient: Applied<br>Resize: Fill (center crop) 320x320                                      | Same as Version 10                                                                                                                                                            |
| 12      | --           | --                                                | --                                                                                              | --                                                                                                                                                                            |
| 13      | 783          | Train Set: 723<br>Valid Set: 30<br>Test Set: 30   | Auto-Orient: Applied<br>Resize: Fill (center crop) 160x160                                      | Same as Version 10                                                                                                                                                            |
| 14      | 781          | Train Set: 721<br>Valid Set: 30<br>Test Set: 30   | Auto-Orient: Applied<br>Resize: Stretch to 160x160                                              | Same as Version 10                                                                                                                                                            |
| 15      | 783          | Train Set: 723<br>Valid Set: 30<br>Test Set: 30   | Auto-Orient: Applied<br>Resize: Fit within 160x160                                              | Same as Version 10                                                                                                                                                            |
| 16      | 782          | Train Set: 722<br>Valid Set: 30<br>Test Set: 30   | Auto-Orient: Applied<br>Resize: Stretch to 96x96                                                | Same as Version 10                                                                                                                                                            |
| 17      | 782          | Train Set: 722<br>Valid Set: 30<br>Test Set: 30   | Auto-Orient: Applied<br>Resize: Fill (center crop) 96x96                                        | Same as Version 10                                                                                                                                                            |
| 18      | 901          | Train Set: 826<br>Valid Set: 40<br>Test Set: 35   | Auto-Orient: Applied<br>Resize: Stretch to 160x160                                              | Same as Version 10                                                                                                                                                            |
| 19      | 903          | Train Set: 828<br>Valid Set: 40<br>Test Set: 35   | Auto-Orient: Applied<br>Resize: Stretch to 320x320                                              | Same as Version 10                                                                                                                                                            |
| 20      | 903          | Train Set: 828<br>Valid Set: 40<br>Test Set: 35   | Auto-Orient: Applied<br>Resize: Stretch to 224x224                                              | Same as Version 10                                                                                                                                                            |
| 21      | 902          | Train Set: 827<br>Valid Set: 40<br>Test Set: 35   | Auto-Orient: Applied<br>Resize: Stretch to 288x288                                              | Same as Version 10                                                                                                                                                            |
| 22      | 1141         | Train Set: 1036<br>Valid Set: 60<br>Test Set: 45  | Auto-Orient: Applied<br>Resize: Stretch to 224x224                                              | Same as Version 10                                                                                                                                                            |
| 23      | 1142         | Train Set: 1037<br>Valid Set: 60<br>Test Set: 45  | Auto-Orient: Applied<br>Resize: Fill (center crop) 224x224                                      | Same as Version 10                                                                                                                                                            |
| 24      | 1143         | Train Set: 1038<br>Valid Set: 60<br>Test Set: 45  | Auto-Orient: Applied<br>Resize: Stretch to 256x256                                              | Same as Version 10                                                                                                                                                            |
| 25      | 1142         | Train Set: 1037<br>Valid Set: 60<br>Test Set: 45  | Auto-Orient: Applied<br>Resize: Stretch to 256x256                                              | Same as Version 10                                                                                                                                                            |
| 26      | 1142         | Train Set: 1038<br>Valid Set: 60<br>Test Set: 45  | Auto-Orient: Applied<br>Static Crop: 25-75% Horizontal & Vertical<br>Resize: Stretch to 256x256 | Same as Version 10                                                                                                                                                            |
| 27      | 451          | Train Set: 346<br>Valid Set: 60<br>Test Set: 45   | Auto-Orient: Applied<br>Static Crop: 25-75% Horizontal & Vertical<br>Resize: Stretch to 256x256 | No augmentations                                                                                                                                                              |
| 28      | 451          | Train Set: 451                                    | Auto-Orient: Applied<br>Static Crop: 25-75% Horizontal & Vertical<br>Resize: Stretch to 256x256 | No augmentations                                                                                                                                                              |
| 29      | 451          | Train Set: 451                                    | Auto-Orient: Applied<br>Resize: Stretch to 256x256                                              | No augmentations                                                                                                                                                              |
| 30      | 1209         | Train Set: 1049<br>Valid Set: 60<br>Test Set: 100 | Auto-Orient: Applied<br>Resize: Stretch to 256x256                                              | Outputs per training example: 3<br>Flip: Horizontal, Vertical<br>90° Rotate CW/CCW<br>Rotation: ±15°                                                                          |

---

## 📌 Notes:

* Some versions focused on testing specific **image sizes** (32×32, 96×96, 160×160, etc.).
* Others evaluated different **augmentation strategies** (flipping, rotation, brightness, noise, etc.).
* The **final version used for mobile app deployment was Version 30**.

---

## 📥 Dataset Access

The dataset is available on **Roboflow**:
👉 [https://app.roboflow.com/trabalho-ecc6m/typecoffee](https://app.roboflow.com/trabalho-ecc6m/typecoffee)

---

## 📜 License

This dataset is released under the **GNU GPL-3.0 License**.
See the root repository `LICENSE` file for details.

---
