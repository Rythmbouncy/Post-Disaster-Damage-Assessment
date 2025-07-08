#  Earthquake Damage Assessment using Transfer Learning

This project uses satellite imagery from the xBD dataset to automatically classify the extent of building damage after an earthquake using deep learning and transfer learning techniques.


---

##  Problem Statement

After natural disasters, rapid and accurate damage assessment is critical. Manual analysis of satellite images is time-consuming. This project builds a machine learning model to **classify damage levels** of buildings (e.g., *no damage, minor, severe*) using **paired pre- and post-disaster images**.

---

##  Dataset

- **Source**: [xBD Dataset](https://xview2.org/)
- **Subset Used**: Mexico Earthquake
- **Input**: Cropped satellite images of individual buildings before and after the earthquake.
- **Labels**:
  - `no-damage`
  - `minor-damage`
  - `severe-damage`
 

---

## 🛠️ Tech Stack

| Area                  | Tools/Technologies             |
|-----------------------|-------------------------------|
| Programming Language  | Python                        |
| Deep Learning         | PyTorch / torchvision         |
| Model Architecture    | ResNet50 (ImageNet weights)   |
| Cloud Platform        | Kaggle Notebooks (GPU)        |
| Image Processing      | OpenCV, PIL                   |
| Data Handling         | Pandas, CSV, os               |
| Evaluation            | Accuracy, F1-Score, Confusion Matrix |

---

##  How It Works

1. **Preprocessing**: Pairs pre- and post-disaster images and labels them using folder structure.
2. **Transfer Learning**: Fine-tunes ResNet50 for 4-class damage classification.
3. **Training**: Trains on paired image inputs using a custom PyTorch Dataset.
4. **Evaluation**: Uses metrics like accuracy and confusion matrix to assess performance.

---

##  Running on Kaggle

1. **Upload or place the repository contents** into a Kaggle Notebook workspace (Don't Forget to Upload the Dataset!)
3. Open `final.ipynb` and run the cells to:
- Generate the `paired_buildings.csv`
- Train the model
- Evaluate results

4. Make sure your Kaggle notebook has **GPU enabled** (Settings → Accelerator → GPU).

---


##  Future Improvements

- Add Grad-CAM visualizations for interpretability
- Explore EfficientNet or Vision Transformers
- Try segmentation models for pixel-level damage detection
- Address class imbalance using weighted loss or focal loss

---

##  License & Credits

- Dataset: [xBD by DIU & Maxar](https://xview2.org/)
- Model: Based on pretrained ResNet from PyTorch
- Author: [Rythmbouncy](https://github.com/Rythmbouncy)

---






