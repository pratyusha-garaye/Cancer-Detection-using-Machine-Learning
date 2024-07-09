# Breast Cancer Prediction using Scikit-Learn and Seaborn 

### 1. Software used
* Python with ML Libraries installed
* VS Code Environmet


### 2. Required Dataset
[Source](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data) - Kaggle

#### Attribute Information:
1.	ID number
2.	Diagnosis (M = malignant, B = benign)

* (3 – 32)
Ten real-valued features are computed for each cell nucleus:
1. radius (mean of distances from center to points on the perimeter)
2. texture (standard deviation of gray-scale values)
3. perimeter
4. area
5. smoothness (local variation in radius lengths)
6. compactness (perimeter^2 / area - 1.0)
7. concavity (severity of concave portions of the contour)
8. concave points (number of concave portions of the contour)
9. symmetry
10. fractal dimension ("coastline approximation" - 1)

* The mean, standard error and "worst" or largest (mean of the three largest values) of these features were computed for each image, resulting in 30 features. For instance, field 3 is Mean Radius, field 13 is Radius SE, field 23 is Worst Radius.
* All feature values are recoded with four significant digits.

* Headers of the dataset:
<img width="1067" alt="Screenshot 2024-07-07 at 12 15 05 AM" src="https://github.com/pratyusha-garaye/Cancer-Detection-using-Machine-Learning/assets/172596779/62d1b09d-0d84-4551-a9f8-dc498878a305">

### 3. EDA and Label Encoding
* Exploratory data analysis was performed using Pandas. Column with missing values was dropped.
* Categorical variable is converted to numerical values.

### 4. Cancer Prediction using Logistic Regression 
* Dataset is split into training and test set. 75% of the data was used for training while remaining 25% was used for test.
* Logistic Regression package is imported from Scikit-Learn and applied to get prediction on the presence of cancer.
* The predicted values is plotted as a heatmap of the Confusion Matrix using Seaborn Library to determine the number of Type I and Type II errors. 

* Confusion Matrix :
![Confusion Matrix](https://github.com/pratyusha-garaye/Cancer-Detection-using-Machine-Learning/assets/172596779/8e6c6070-04ea-4c83-9e1a-cfee0afd9a44)

### Calculated accuracy_score of the prediction: 97.89%
