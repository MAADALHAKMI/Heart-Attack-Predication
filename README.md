# 🧠 Heart Attack Prediction using Neural Networks (with TensorFlow)

This project is a heart attack prediction model built using Python and neural networks (TensorFlow/Keras). It uses patient data to predict the likelihood of having a heart attack. The model is trained on structured health data and leverages deep learning for binary classification.

---

## 📁 Project Overview

- **Language:** Python  
- **Libraries Used:** TensorFlow, Scikit-learn, Pandas, NumPy  
- **Algorithm:** Feedforward Neural Network  
- **Use Case:** Predict risk of heart attack (binary output: likely/unlikely)

---

## 🧠 Model Architecture

```
Input Layer → Dense(32, ReLU) → Dense(16, ReLU) → Output Layer (1, Sigmoid)
```

- The model is compiled using:
  - **Loss function:** Binary Crossentropy
  - **Optimizer:** Adam
  - **Metrics:** Accuracy

---

## 📊 Dataset

The dataset is expected in **CSV format** and must include the following features (13 columns total), with the last column named `output` (the target label).

**Note:** You must update the file path in the script before running the model:

```python
file_path = r"C:\Users\your_path\heart.csv"
```

Replace it with your own local path to the `heart.csv` dataset.

---

## ⚙️ How to Run

### 1. Install Requirements

```bash
pip install -r requirements.txt
```

### 2. Run the Model

```bash
python heart_model.py
```

The script will:
- Load and preprocess the data
- Train a neural network
- Evaluate its accuracy
- Allow predictions on new data

---

## 🔍 Predicting New Data

You can predict new samples in two ways:

### ➤ 1. Hardcoded Example:
Change the values in the list below to test:

```python
new_data = [[52, 1, 0, 125, 212, 0, 1, 168, 0, 1.0, 1, 2, 2]]
```

### ➤ 2. Interactive Input (Command-Line):
The script will ask you to enter 13 values manually with descriptions in Arabic.

---

## 🧪 Output Example

```
Epoch 100: Train Accuracy = 0.92, Validation Accuracy = 0.89

Accuracy on test data: 0.91

Classification Report:
              precision    recall  f1-score   support
           0       0.90      0.95      0.92        60
           1       0.92      0.85      0.88        50
```

---

## 🛠 Future Improvements

- Export trained model for deployment
- Add Flask or Streamlit interface for web use
- Enhance dataset and handle imbalanced data
- Add cross-validation

---

## 📝 Notes

- This project is for educational purposes.
- Always validate medical predictions with professional healthcare providers.

---

## 📂 File Structure

```
├── heart_model.py          # Main code
├── heart.csv               # Dataset (your data if you have  )
├── README.md               # Project documentation
└── requirements.txt        # Python dependencies
```

---

## 📧 Contact

For questions or suggestions, feel free to reach out or fork the repository!
