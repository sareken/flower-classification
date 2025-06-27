# flower-classification-cnn

This project is a deep learning-based flower classification system trained on the Oxford 17 Category Flower Dataset. Various CNN architectures were tested, with MobileNetV2 providing the best balance of accuracy and performance. The models were trained using data augmentation and saved in `.keras` format. Final evaluation included both numeric metrics and visual analysis.

---

## Features

- Image classification using MobileNetV2, ResNet50, and CBAM-enhanced ResNet50
- Preprocessing with `ImageDataGenerator` and `flow_from_dataframe`
- Extensive data augmentation applied during training
- EarlyStopping and learning rate scheduling to prevent overfitting
- Final models saved in `.keras` format
- Visual and numerical evaluation of model performance

---

## Technologies Used

- Python
- TensorFlow / Keras
- Pre-trained CNNs: MobileNetV2, ResNet50
- CBAM attention module (custom layer)
- Matplotlib, Seaborn
- Pandas, NumPy
- Scikit-learn

---

## Files and Descriptions

| File Name | Description |
|-----------|-------------|
| `mobilenetv2_final_best.keras` | Best performing lightweight model |
| `final_resnet_flowers17.keras` | Standard ResNet50-based model |
| `labels.mat` | MATLAB file containing class labels |
| `Untitled-1.ipynb` | Full training and evaluation notebook |

---

## Training Details

- Input shape: `224x224x3`
- Optimizer: Adam (learning rate = 1e-4)
- Loss Function: Categorical Crossentropy
- Callbacks: EarlyStopping, ReduceLROnPlateau, ModelCheckpoint
- Epochs: Up to 40 with patience of 5
- Batch size: 32
- Data Split: 70% training, 15% validation, 15% test
- Data augmentation:
  - Rotation, shifting, zoom, brightness, horizontal flip

---

## How to Run

Install the required libraries:

```bash
pip install tensorflow matplotlib pandas numpy pillow seaborn scipy
```
![](karsilastirma.pnj)
