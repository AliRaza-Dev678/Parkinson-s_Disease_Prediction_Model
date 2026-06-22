# 🧠 Parkinson's Disease Prediction Model

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=flat-square&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat-square&logo=jupyter)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-yellowgreen?style=flat-square&logo=scikit-learn)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)

A machine learning model that predicts the presence of **Parkinson's Disease** in patients using biomedical voice measurements. Built with Python and scikit-learn, this project demonstrates an end-to-end ML pipeline — from data preprocessing to model evaluation.

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Dataset](#-dataset)
- [Features](#-features)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [Usage](#-usage)
- [Model Performance](#-model-performance)
- [Technologies Used](#-technologies-used)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🔍 Overview

Parkinson's Disease is a progressive neurological disorder that affects movement. Early detection is crucial for managing symptoms and improving patient quality of life. This project leverages **voice measurement features** — since vocal impairment is one of the earliest symptoms — to classify whether a person has Parkinson's Disease or not.

The model is trained on the well-known **Oxford Parkinson's Disease Detection Dataset** and achieves high classification accuracy using supervised learning techniques.

---

## 📊 Dataset

| Property | Details |
|---|---|
| **Source** | UCI Machine Learning Repository |
| **File** | `parkinsons.csv` |
| **Samples** | 195 voice recordings |
| **Features** | 22 biomedical voice measurements |
| **Target** | `status` (1 = Parkinson's, 0 = Healthy) |
| **Class Distribution** | ~75% Parkinson's, ~25% Healthy |

### Key Features in the Dataset

| Feature | Description |
|---|---|
| `MDVP:Fo(Hz)` | Average vocal fundamental frequency |
| `MDVP:Fhi(Hz)` | Maximum vocal fundamental frequency |
| `MDVP:Flo(Hz)` | Minimum vocal fundamental frequency |
| `MDVP:Jitter(%)` | Variation in fundamental frequency |
| `MDVP:Shimmer` | Variation in amplitude |
| `NHR`, `HNR` | Noise-to-harmonics ratios |
| `RPDE`, `DFA` | Nonlinear dynamical complexity measures |
| `spread1`, `spread2`, `D2`, `PPE` | Nonlinear measures of fundamental frequency variation |

---

## ✨ Features

- **Data Preprocessing** — Handles feature scaling and normalization
- **Exploratory Data Analysis (EDA)** — Correlation heatmaps, class distribution plots, and feature analysis
- **Model Training** — Trains and compares multiple classification algorithms
- **Model Evaluation** — Confusion matrix, accuracy, precision, recall, and F1-score
- **Prediction Pipeline** — Ready-to-use prediction on new input data

---

## 📁 Project Structure

```
Parkinson-s_Disease_Prediction_Model/
│
├── Parkinson_Disease_Prediction_Model.ipynb   # Main notebook with full pipeline
├── parkinsons.csv                              # Dataset
└── README.md                                   # Project documentation
```

---

## ⚙️ Installation

### Prerequisites

Make sure you have **Python 3.8+** installed. Then clone this repository and install the required libraries.

```bash
# Clone the repository
git clone https://github.com/AliRaza-Dev678/Parkinson-s_Disease_Prediction_Model.git
cd Parkinson-s_Disease_Prediction_Model
```

### Install Dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

Or install all at once using:

```bash
pip install -r requirements.txt
```

> **Tip:** It is recommended to use a virtual environment:
> ```bash
> python -m venv venv
> source venv/bin/activate      # On Linux/macOS
> venv\Scripts\activate         # On Windows
> ```

---

## 🚀 Usage

1. Launch Jupyter Notebook:

```bash
jupyter notebook
```

2. Open `Parkinson_Disease_Prediction_Model.ipynb` in your browser.

3. Run all cells sequentially (`Cell → Run All`) to:
   - Load and explore the dataset
   - Preprocess features
   - Train the model
   - Evaluate performance
   - Make predictions

### Making a Prediction

To predict on new data, provide a row of 22 biomedical voice measurements in the format of the dataset and run the prediction cell at the bottom of the notebook.

---

## 📈 Model Performance

The model is evaluated using standard classification metrics:

| Metric | Score |
|---|---|
| **Accuracy** | ~95% |
| **Precision** | High |
| **Recall** | High |
| **F1-Score** | High |

> Exact scores are printed in the notebook output after running all cells.

---

## 🛠️ Technologies Used

| Tool | Purpose |
|---|---|
| **Python 3** | Core programming language |
| **Jupyter Notebook** | Interactive development environment |
| **NumPy** | Numerical computation |
| **Pandas** | Data manipulation and analysis |
| **Matplotlib / Seaborn** | Data visualization |
| **scikit-learn** | Machine learning algorithms and evaluation |

---

## 🤝 Contributing

Contributions are welcome! If you have suggestions to improve the model, add new features, or fix issues:

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m "Add: your feature description"`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** — you are free to use, modify, and distribute it with proper attribution.

---

## 👨‍💻 Author

**Ali Raza**
- GitHub: [@AliRaza-Dev678](https://github.com/AliRaza-Dev678)

---

## 🙏 Acknowledgements

- **UCI Machine Learning Repository** for providing the Oxford Parkinson's Disease Detection Dataset
- Max A. Little of the University of Oxford for the original dataset collection

---

> ⚠️ **Disclaimer:** This project is intended for educational and research purposes only. It is **not** a medical diagnostic tool and should not be used as a substitute for professional medical advice.
