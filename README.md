# ⚡ Power Plant Energy Output Prediction using ANN
## 📌 Overview

This project implements an Artificial Neural Network (ANN) using PyTorch to predict the electrical energy output of a power plant based on environmental conditions such as temperature, pressure, humidity, and exhaust vacuum.

The model achieves an **R² Score of 0.93**, meaning it predicts power plant energy output with 93% accuracy.

---

## 🎯 Objective

To predict the electrical energy output (PE) of a combined cycle power plant using deep learning techniques, helping improve energy forecasting and operational efficiency.

---

## 📊 Dataset

The dataset contains the following features collected from a power plant over 6 years:

| Feature | Description |
|---------|-------------|
| AT | Ambient Temperature (°C) |
| V | Exhaust Vacuum (cm Hg) |
| AP | Ambient Pressure (millibar) |
| RH | Relative Humidity (%) |
| PE | Electrical Energy Output - Target Variable (MW) |

---

## 🛠️ Technologies Used

- **Python 3.x**
- **PyTorch** — Neural Network building and training
- **Pandas** — Data loading and manipulation
- **NumPy** — Numerical computations
- **Scikit-Learn** — Preprocessing and evaluation metrics
- **Matplotlib** — Visualization
- **Jupyter Notebook** — Development environment

---

## 🧠 ANN Architecture

```
Input Layer  →  4 features (AT, V, AP, RH)
     ↓
Hidden Layer 1  →  6 Neurons  →  ReLU Activation
     ↓
Hidden Layer 2  →  6 Neurons  →  ReLU Activation
     ↓
Output Layer  →  1 Neuron  →  Predicted Energy Output (PE)
```

---

## ⚙️ Training Configuration

| Parameter | Value |
|-----------|-------|
| Optimizer | Adam |
| Loss Function | Mean Squared Error (MSE) |
| Epochs | 100 |
| Batch Size | 32 |

---

## 📈 Results

| Metric | Value |
|--------|-------|
| **R² Score** | **0.9314** |
| MSE | — |
| RMSE | — |
| MAE | — |

> The model achieves **93.14% accuracy** in predicting power plant energy output!

---

## 🔧 Data Preprocessing

- Data Loading using Pandas
- Feature Selection (AT, V, AP, RH as inputs)
- Train-Test Split (80/20)
- Feature Scaling using **StandardScaler**
- Conversion to PyTorch Tensors

---

## 🚀 Project Workflow

1. Load Power Plant Dataset
2. Explore and understand the data
3. Split into Training and Testing sets
4. Standardize features using StandardScaler
5. Convert data to PyTorch Tensors
6. Build ANN Model architecture
7. Train the model for 100 epochs
8. Evaluate performance using R², MSE, RMSE, MAE
9. Visualize Actual vs Predicted output

---

## 📂 Project Structure

```
powerplant/
│
├── ann.ipynb           ← Main notebook with full code
├── best_model.pt       ← Saved trained model
├── requirements.txt    ← Dependencies
└── README.md           ← Project documentation
```

---

## 📥 Installation & Usage

**Clone the repository:**
```bash
git clone https://github.com/shaik-zabi-321/ann-regression.git
cd ann-regression
```

**Install dependencies:**
```bash
pip install -r requirements.txt
```

**Launch Jupyter Notebook:**
```bash
jupyter notebook
```

Open `ann.ipynb` and run all cells.

---

## 📦 Requirements

```
torch
pandas
numpy
scikit-learn
matplotlib
jupyter
```

---

## 📈 Applications

- Energy Forecasting
- Power Plant Optimization
- Industrial Automation
- Resource Management
- Performance Monitoring

---

## 🔮 Future Improvements

- Hyperparameter Tuning with Grid Search
- Deeper Neural Network architectures
- Model Deployment using Flask or FastAPI
- Real-Time Prediction Dashboard
- Comparison with Traditional Regression Models (Linear, Random Forest)

---

## 👨‍💻 Author

**Shaik Zabiulla**
B.Tech Artificial Intelligence
Rayalaseema University College of Engineering, Kurnool



---

## 📜 License

This project is intended for educational and research purposes.

---

> ⭐ If you found this project helpful, please give it a star on GitHub!
