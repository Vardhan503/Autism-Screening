## [Abstract](#table-of-contents)
Improve Autism Screening by developing a model that predicts the likelihood of having this disorder.

## [What is Autism?](#table-of-contents)
Autism spectrum disorder (ASD) is a developmental impairment caused by abnormalities in the brain. People with ASD may struggle with confined or repetitive activities or interests, as well as social communication and engagement. Additionally, people with ASD may learn, move, or pay attention in various ways.

## [Related Resources](#table-of-contents)
- Medium Blog: [Autism Spectrum Disorder Prediction Using Artificial Neural Networks](https://medium.com/@vardhansaireddy1245/predicting-autism-screening-using-ann-e18ba78802b5)

# Table of contents

- [Abstract](#Abstract)
- [What is Autism?](#What-is-Autism?)
- [Related Resources](#Related-Resources)
- [Installation](#table-of-contents)
- [Implementation](#Implementation)
- [Conclusion](#Conclusion)
- [Adding new features](#Adding-new-features)

Python 3.9 was used to create the application files. Before running the files, it must be ensured that Python 3.9 and the following libraries are installed.

| Library  | Task |
| ------------- | ------------- |
| [Numpy](https://numpy.org/install/)  | Mathematical Operations  |
| [Pandas](https://pandas.pydata.org/docs/getting_started/install.html)  | Data Analysis Tools  |
| [Matplotlib](https://matplotlib.org/stable/users/installing/index.html)  | Visualizations  |
| [Sklearn](https://scikit-learn.org/stable/install.html)  | Machine Learning Library  |
| [Tensorflow](https://www.tensorflow.org/install)  | Modelling  |
| [Ploty](https://plotly.com/python/getting-started/)  | Graphical Visualizations  |


# [Implementation](#table-of-contents)

**Download dataset**


1. Data Preprocessing: We will prepare our dataset for analysis in this part:
    - Importing libraries.
    - Reading Data.
    - Verify any missing data.
    - Evaluate the DataFrame's Shape.
    - Review dataset statistics.
    - Examining the dataset's feature datatypes.
    - Checking for outliers and removing them.
    - Ethnicity and relation contains ? values which are invalid and others, Others both are same, so replace them with Others.
    - Exploring correlations between the elements using ploty and matplotlib visualisations.
    - Dropping unwanted columns
    - Splitting Data into x and y
    - Change the categorical columns to the numerical columns
    - Divide the data into train and test sets.

2. Creation of an ANN Model
    - Adding input, hidden, and output layers, and constructing a sequential model. 
    - Adam optimizer and binary cross entropy ought to be used to train the model.
    - Early stopping is used, allowing you to define a large number of training epochs at your discretion and end training once the model's performance on a hold out validation dataset stops improving.
    - Evaluation of the model: Using the test dataset, the accuracy score and confusion matrix are assessed.

Each of these steps contained in model_implementation.ipynb file. The file with the ipynb extension has the advantage of saving the state of the last run of that file and the screen output.

Thus, screen output can be seen without re-running the files. Files with the ipynb extension can be run using the [jupyter notebook](https://jupyter.org/) program. When running the codes, the sequence numbers in the filenames should be followed.

Because the output of almost every step is the prerequisite for the operation of the next step. 

### [Conclusion](#table-of-contents)
Our trained model's total classification accuracy while using test data is 0.95. It should be noted that this quantity reflects perfect classification. In reality, other models that focus on Class/ASD label binary classification may obtain higher accuracy of ideal classification.

### [Adding new features](#table-of-contents)

In order to make even more advancements, we can train our model using a variety of classification algorithms, including Logistic Regression, Naive Bayes, SVM, KNN, Random Forest, and AdaBoost. Based on a comparison analysis of performance metrics, we can choose the algorithm that is best for classifying autism in autism screenings.
