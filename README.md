# CodeAlpha_Handwritten-character-recognition
# EMNIST + MNIST CNN Classifier

This project combines the **MNIST** (digits) and **EMNIST Letters** datasets to train a CNN model that classifies handwritten digits (0–9) and uppercase letters (A–Z) using TensorFlow and Keras.

---

## 📦 Dataset

- **MNIST**: Loaded using `tensorflow.keras.datasets.mnist`.
- **EMNIST Letters**: Downloaded from Kaggle using `kagglehub`. You must have your Kaggle API key configured.

---

## 🔧 Setup Instructions

### 1. Install Dependencies

```bash
pip install numpy pandas matplotlib seaborn tensorflow scikit-learn kagglehub

Ensure you have your kaggle.json API key file placed correctly:
mkdir ~/.kaggle
cp kaggle.json ~/.kaggle/
chmod 600 ~/.kaggle/kaggle.json

 Run the Script
python train_model.py

Label Mapping
Digits: 0–9
Letters: 10–35 → A–Z
Total of 36 classes.

Evaluation
Training/Validation Accuracy is plotted.
Final test performance is printed, along with a classification report.
Sample predictions are shown for visual inspection.

Example Output
Test Accuracy: 0.9745
Sample Predictions:
True: 0, Predicted: 0
True: A, Predicted: A
True: 9, Predicted: 9

File Structure
.
├── train_model.py         # Main script
├── best_model.keras       # Saved best model checkpoint
└── README.md              # This file






