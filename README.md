# Basic Temperature Classification

A machine learning project that classifies temperatures as "High" or "Low" using Logistic Regression. The model is trained on synthetic temperature data and can predict whether a given temperature is above or below a threshold of 30°C.

## 📋 Features

- **Binary Classification**: Classifies temperatures as "High" (≥30°C) or "Low" (<30°C)
- **Logistic Regression Model**: Uses scikit-learn's Logistic Regression for classification
- **Data Visualization**: Includes scatter plots and confusion matrix visualization
- **Easy-to-Use Function**: Simple function to classify single or multiple temperatures
- **Model Evaluation**: Comprehensive evaluation with accuracy score and classification report

## 🛠️ Requirements

The following Python packages are required:

- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`
- `seaborn`

## 📦 Installation

1. Clone this repository:
```bash
git clone https://github.com/digambars-git-hub/Basic-Temperature-Classification.git
cd Basic-Temperature-Classification
```

2. Install the required packages:
```bash
pip install -r requirements.txt
```

## 🚀 Usage

### Running the Notebook

1. Open `Temperature_classification.ipynb` in Jupyter Notebook or Google Colab
2. Run all cells sequentially to:
   - Generate synthetic temperature data
   - Train the logistic regression model
   - Evaluate the model performance
   - Visualize the results

### Classifying Temperatures

After training the model, you can use the `classify_temperature()` function to classify new temperatures:

```python
classify_temperature([5, 24, 25, 40, 15.5, 35])
```

**Example Output:**
```
5 classified as : low (High probability : 0.0000)
24 classified as : low (High probability : 0.0004)
25 classified as : low (High probability : 0.0014)
40 classified as : high (High probability : 1.0000)
15.5 classified as : low (High probability : 0.0000)
35 classified as : high (High probability : 0.9978)
```

## 📊 How It Works

1. **Data Generation**: Creates 100 random temperature values between 0°C and 50°C
2. **Labeling**: Assigns labels based on a threshold of 30°C (≥30°C = High, <30°C = Low)
3. **Train-Test Split**: Splits data into 70% training and 30% testing sets
4. **Model Training**: Trains a Logistic Regression model on the training data
5. **Evaluation**: Evaluates the model using accuracy score and classification metrics
6. **Visualization**: Displays scatter plots and confusion matrix

## 📈 Model Performance

The model achieves:
- **Accuracy**: 100% (on the test set)
- **Precision**: 1.00 for both Low and High classes
- **Recall**: 1.00 for both Low and High classes
- **F1-Score**: 1.00 for both Low and High classes

## 📁 Project Structure

```
Basic-Temperature-Classification/
│
├── Temperature_classification.ipynb  # Main Jupyter notebook
└── README.md                         # Project documentation
```

## 🔧 Model Details

- **Algorithm**: Logistic Regression
- **Threshold**: 30°C
- **Training Data**: 70 samples
- **Test Data**: 30 samples
- **Random State**: 42 (for reproducibility)

## 📝 Notes

- This is a simple binary classification model for educational purposes
- The model uses synthetic data generated randomly
- The threshold of 30°C can be adjusted in the notebook
- The model achieves perfect accuracy due to the clear separation at the threshold

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 📄 License

This project is open source and available under the MIT License.

## 👤 Author

Your Name

---

⭐ If you find this project helpful, please consider giving it a star!
