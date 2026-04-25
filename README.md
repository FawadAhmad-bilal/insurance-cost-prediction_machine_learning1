# 🏥 Insurance Premium Prediction using Machine Learning

A machine learning project that predicts insurance premiums based on various customer attributes using regression models.

## 📋 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Model Performance](#model-performance)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

This project implements a machine learning model to predict insurance premiums based on customer demographics and health factors. The model helps insurance companies determine appropriate premium amounts by analyzing patterns in historical data.

**Key Objectives:**
- Predict insurance costs accurately using customer features
- Compare multiple regression algorithms
- Provide insights into factors affecting insurance premiums

## ✨ Features

- **Data Preprocessing**: Handles missing values, outliers, and categorical encoding
- **Feature Engineering**: Creates meaningful features from raw data
- **Multiple Models**: Implements and compares various regression algorithms
- **Model Evaluation**: Comprehensive performance metrics (MAE, RMSE, R²)
- **Visualization**: Clear charts showing predictions vs actual values
- **Scalable Pipeline**: Easy to retrain with new data

## 📊 Dataset

The dataset includes the following features:

| Feature | Description | Type |
|---------|-------------|------|
| Age | Customer's age | Numeric |
| Sex | Gender (male/female) | Categorical |
| BMI | Body Mass Index | Numeric |
| Children | Number of dependents | Numeric |
| Smoker | Smoking status (yes/no) | Categorical |
| Region | Geographic region | Categorical |
| Charges | Insurance premium (target) | Numeric |

**Dataset Size**: ~1,338 records

## 🛠️ Technologies Used

- **Python 3.8+**
- **NumPy**: Numerical computations
- **Pandas**: Data manipulation and analysis
- **Matplotlib & Seaborn**: Data visualization
- **Scikit-learn**: Machine learning algorithms
- **Jupyter Notebook**: Interactive development

## 📥 Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Setup Steps

1. Clone the repository
```bash
git clone https://github.com/yourusername/insurance-prediction.git
cd insurance-prediction
```

2. Create a virtual environment (recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required packages
```bash
pip install -r requirements.txt
```

## 🚀 Usage

### Running the Jupyter Notebook

```bash
jupyter notebook insurance_prediction.ipynb
```

### Training the Model

```python
# Load the data
import pandas as pd
df = pd.read_csv('insurance.csv')

# Run preprocessing and training
# (See notebook for detailed steps)
```

### Making Predictions

```python
# Example prediction
new_data = {
    'age': 30,
    'sex': 'male',
    'bmi': 25.5,
    'children': 2,
    'smoker': 'no',
    'region': 'northwest'
}

predicted_premium = model.predict(new_data)
print(f"Predicted Premium: ${predicted_premium:.2f}")
```

## 📈 Model Performance

| Model | MAE | RMSE | R² Score |
|-------|-----|------|----------|
| Linear Regression | $4,200 | $6,100 | 0.75 |
| Random Forest | $2,800 | $4,500 | 0.86 |
| Gradient Boosting | $2,600 | $4,200 | 0.88 |

*Note: Replace with your actual metrics*

## 📁 Project Structure

```
insurance-prediction/
│
├── data/
│   └── insurance.csv          # Dataset
│
├── notebooks/
│   └── insurance_prediction.ipynb  # Main notebook
│
├── src/
│   ├── preprocessing.py       # Data preprocessing functions
│   ├── models.py             # Model training functions
│   └── utils.py              # Utility functions
│
├── models/
│   └── trained_model.pkl     # Saved model
│
├── requirements.txt          # Dependencies
├── README.md                # This file
└── LICENSE                  # License file
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Fawad**
- Student ID: F24-3079
- University of Haripur, Department of Information Technology
- BSAI 4th Semester

## 🙏 Acknowledgments

- Dataset source: [Kaggle Insurance Dataset](https://www.kaggle.com/)
- Inspired by real-world insurance premium calculation problems
- Thanks to instructors and peers for guidance

## 📧 Contact

For questions or suggestions, feel free to reach out or open an issue!

---

⭐ If you find this project helpful, please consider giving it a star!
