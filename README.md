
# Heart Disease Prediction

This project predicts heart disease using the UCI Heart Disease dataset.

## Dataset
- Source: [UCI Heart Disease Dataset](https://www.kaggle.com/ronitf/heart-disease-uci)
- Size: 303 samples, 14 features

## Preprocessing
- Replaced 99 zero values in `oldpeak` with mean (~1.544118).
- Normalized columns

## Model
- **Architecture**: Neural Network with 3 layers (16, 8, 1)
  - Input: ReLU activation, Dropout (0.3)
  - Hidden: ReLU activation, Dropout (0.3)
  - Output: Sigmoid activation
- **Optimizer**: Adam (learning rate = 0.001)
- **Loss**: Binary Crossentropy
- **Training**: 50 epochs with Early Stopping (patience=5)
- **Results**:
- Test accuracy: ~75-80%(depending on features).
- Validation accuracy: ~80-85%.

## Requirements
```bash
pip install pandas numpy scikit-learn

