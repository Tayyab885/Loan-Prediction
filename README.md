# Loan Prediction

This is a repository containing a Jupyter notebook with a machine learning model to predict loan approvals.
The goal of this project is to build a model that can predict whether a loan application will be approved or not, based on a set of features such as the applicant's income, credit history, and loan amount.

## Liabraries
The notebook uses the following libraries:
- NumPy
- Pandas
- Seaborn
- Matplotlib
- Scikit-learn
You can install them using pip.

## Getting Started
To get started with this project, you will need to have Python 3.10 and Jupyter Notebook installed on your system. You can install Jupyter Notebook using pip:
### Clone the repository:
```shell
$ git clone https://github.com/Tayyab885/Loan-Prediction.git
```
Navigate to the directory where the repository was cloned and open the Jupyter notebook:
```shell
$ cd Loan-Prediction
$ jupyter notebook loan_prediction.ipynb
```
## Data Cleaning and Visualization
- The notebook first handles missing values in both the train and test datasets using the mode and mean, respectively. Then, the notebook uses data visualization techniques to better understand the data.
- For categorical features, a countplot is used to show the distribution of values. For numerical features, a histogram is used to show the distribution of values. Next, a bar graph is used to show the relationship between each categorical feature and the target feature (Loan_Status). Finally, a boxplot is used to show the relationship between each numerical feature and the target feature.
- After visualizing the data, outliers in numerical features are removed using the interquartile range (IQR) method. The notebook then uses label encoding to convert categorical features to numerical features using the map function.

## Model Training and Prediction
- The notebook splits the data into training and testing sets and trains a random forest tree classifier using Scikit-learn. The notebook achieves 80% accuracy on the test dataset.
- Finally, the notebook uses label encoding to convert categorical features in the test dataset to numerical features and predicts the target feature (Loan_Status) using the trained classifier.
