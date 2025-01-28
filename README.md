# Breast Cancer Classification with SVM

This project demonstrates the use of a Support Vector Machine (SVM) classifier to predict breast cancer.

## Dataset

The project utilizes the Breast Cancer Wisconsin (Diagnostic) Dataset, which is a classic dataset for binary classification. The dataset contains features computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. These features describe characteristics of the cell nuclei present in the image.

**Features:**

The dataset includes 30 features, such as:

* radius (mean of distances from center to points on the perimeter)
* texture (standard deviation of gray-scale values)
* perimeter
* area
* smoothness (local variation in radius lengths)
* compactness (perimeter^2 / area - 1.0)
* concavity (severity of concave portions of the contour)
* concave points (number of concave portions of the contour)
* symmetry
* fractal dimension ("coastline approximation" - 1)

**Target Variable:**

* Diagnosis (M = malignant, B = benign)

## Methodology

1. **Data Loading:** The Breast Cancer Wisconsin dataset is loaded using scikit-learn's `datasets.load_breast_cancer()` function.
2. **Data Splitting:** The dataset is split into training and testing sets using `train_test_split()` with a test size of 20% and a random state of 42 for reproducibility.
3. **Feature Scaling:** Features are scaled using `StandardScaler()` to ensure that all features have a similar range of values.
4. **SVM Classifier:** An SVM classifier with a linear kernel and a regularization parameter (C) of 1 is trained on the scaled training data.
5. **Predictions:** Predictions are made on the scaled testing data using the trained SVM classifier.
6. **Evaluation:** The model's performance is evaluated using accuracy score, confusion matrix, and classification report.
7. **Visualization:** Principal Component Analysis (PCA) is used to reduce the dimensionality of the data to 2 components for visualization purposes. The training data points and the decision boundary of the SVM classifier are plotted.

## Results

The accuracy, confusion matrix, and classification report are printed to the console.

To see the output, run the code.

## Dependencies

* Python 3.x
* NumPy
* Matplotlib
* scikit-learn

## Usage

1. Clone the repository.
2. Install the required dependencies.
3. Run the Jupyter Notebook.
