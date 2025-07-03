# Iris Flower Classification with Machine Learning

This project demonstrates how to classify iris flowers into three species (Setosa, Versicolor, Virginica) using their measurements with a machine learning model.

## Dataset

The dataset consists of the following columns:
- SepalLengthCm
- SepalWidthCm
- PetalLengthCm
- PetalWidthCm
- Species

You can use the provided `Iris.csv` file.

## Requirements

- Python 3.x
- pandas
- scikit-learn

Install dependencies with:
```sh
pip install pandas scikit-learn
```

## How to Run

1. Place the `Iris.csv` file in the same folder as the script.
2. Run the script:

```sh
python iris_classification.py
```

## What the Script Does

- Loads and preprocesses the data (removes `Id` column, encodes `Species`).
- Splits the data into training and testing sets.
- Trains a Random Forest classifier.
- Evaluates the model (prints accuracy and classification report).
- Predicts the species of a sample flower (you can edit the sample in the script).

## Example Output

```
Accuracy: 1.0

Classification Report:
              precision    recall  f1-score   support

  Iris-setosa       1.00      1.00      1.00        10
Iris-versicolor       1.00      1.00      1.00        10
 Iris-virginica       1.00      1.00      1.00        10

    accuracy                           1.00        30
   macro avg       1.00      1.00      1.00        30
weighted avg       1.00      1.00      1.00        30

Predicted species for sample [[5.1, 3.5, 1.4, 0.2]]: Iris-setosa
```

## Custom Prediction

You can change the values in the `sample` variable in `iris_classification.py` to predict the species for different measurements.

---

**References:**  
- [Scikit-learn documentation](https://scikit-learn.org/stable/)
- [Iris dataset on Wikipedia](https://en.wikipedia.org/wiki/Iris_flower_data_set)
