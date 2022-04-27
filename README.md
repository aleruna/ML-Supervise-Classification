# Sports Analytic :

# Machine Learning Supervise Classification

## Index

- [1.Abstract](#abs)
- [2. Introduction](#intro)
- [3.Dataset](#data)
  - [3.1.Data clean](#data_clean)
  - [3.2 Data analysis](#data_analysis)
- [4. Methods](#methods)
  - [4.1. KNN]
  - [4.2. Naive Bayes]
  - [4.3.Gaussian ]
  - [4.4. Logistic Regression]
- [5. Results](#result)
- [6. Conclusions](#conclusiones)

<a id="abs"> </a>

<h2> 1. Abstract </h2>
<p style="font:10px"> It is a simple project where the main goal is to apply machine learning classification methods to predict if a rookie player will stay over five years. Therefore promote to the professional category.</p>

<a id="intro"></a>

<h2> 2. Introduction </h2>
<p>The National Basket Association (NBA) is one of the most popular and recognized leagues. It is a billion dollars business with millions of viewers around the world. Only in 2018-2019, the combined avenue of teams of the NBA was over 8.7 billion dollars(Nguyen et. al 2021). The main aim of this study is to evaluate the effectiveness of applying Machine Learning (ML) techniques to predict players' future performance, through their primary statistics. To achieve this goal, It will apply basic supervised classification ML methods, such as Dummies Classifier (for establishing a baseline) KNN, Naive Bayes, Logistic Regression, and Random Forrest. The metric score chosen for this project is F1-score and Recall. The score elected take after the recomendation published in "Imbalanced Classification with Python" by Jason Brownle, due to have a classification problem with an imbalanced dataset, a positive class more important.</p>
<p> A sample of 10% of the dataset was taken out for later verification of the predicted models resulting </p>

<a id="data"></a>

<h2>3.Dataset</h2>
Find the repository in the following link https://data.world/exercises/logistic-regression-exercise-1. The dataset can be split into two types of categories, accumulative variables and percentage variables. Also, it contains the target feature label as (target_5yrs).
<a id="data_clean"></a>
<h3> 3.1 Data Clean</h3>
Given the low number of null data, we decided to drop them, which resulted in the loss of eleven samples. Furthermore, duplicates also represent less than 30 samples so they take out the dataset.
<a id="data_analysis"></a>
<h3> 3.2 Data Analysis</h3>
A diagram was made to visualize the correlation between all the features but also how they interact with the target. Also, a few diagrams were add to understanding the data.

<a id="methods"></a>

<h2> 4. Methods </h2>
<p>The target feature was unbalanced, therefore hyperparameter  "stratify" was considered in  "train_test_split" method. Also for every model used in this project GridSearch method was incorporated,"StratifyFold" was also applied in GridSearch with (n_splits=10, random_state=19, shuffle=True) </p><br>

<p>Recall was selected as the scoring target </p>

<a></a>

<h3> 4.1 KNN</h3>
After using gridsearch the best parameters were [Manhattan] and n_neighbords = 13.<br>
<br>
KNN model had a final recall= 0.74 and F1-Score = 0.74

<h3> 4.2 Naive Bayes</h3>
This model resulted in a recall= 0.66 and F1-Score = 0.69<br>

<h3> 4.3 Gaussian Naive Bayes (GaussianNB)</h3>
This model had the lowest result with recall= 0.56 and F1-Score = 0.66 <br>

<h3> 4.4 Loggist regresion</h3>
For this model the following parameters were applied C': 1.0,'class_weight': None,
 'dual': False,'fit_intercept': True,'intercept_scaling': 1, 'l1_ratio': None,
 'max_iter': 100000, 'multi_class': 'auto', 'n_jobs': None, 'penalty': 'none',
 'random_state': None, 'solver': 'lbfgs', 'tol': 0.0001, 'verbose': 0, 'warm_start': False <br>
This model had the best result whit recall= 0.82 and F1-Score = 0.77 <br>

<h2> 5. Results </h2>

|          | KNN  | MultinomialNB | GaussianNB | Reg. Log. | Reg. Modific. |
| -------- | ---- | ------------- | ---------- | --------- | ------------- |
| Recall   | 0.74 | 0.66          | 0.56       | 0.77      | 0.82          |
| F1-Score | 0.74 | 0.69          | 0.66       | 0.74      | 0.77          |

![roc curve](https://github.com/aleruna/ML-Supervise-Classification/blob/main/roc_curve.JPG)

On the other hand, the sample of 10% of the database that had been previously extracted, shows good results with more than 70% of the class predicted.

<h2> 6. Conclusions </h2>
It could conclude that the best model for this project if we are considering the target score, was Loggist Regression.

<p>Disclaimer: I'm not a native english speaker so sorry for any mistake on the text </p>
