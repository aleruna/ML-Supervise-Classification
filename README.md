# rookies_NBA

## Index

- [1.Abstract](#abs)
- [2. Introduction](#intro)
- [3.Dataset](#data)
    - [3.1.Data clean](#data_clean)
    - [3.2 Data analysis](#data_analysis)
 - [4. Methods](#resultados)
    - [4.1. KNN](#KNN)
    - [4.2. Naive Bayes](#NB)
    - [4.3.Gaussian ](#GB)
    - [4.4. Logistic Regression](#RL)
- [5. Results](#resul)
- [6. Conclusions](#conclusiones)

<a id="abs"> </a>
<h2> 1. Abstract </h2>
<p style="font:10px"> It is a simple project where the main goal is to apply machine learning classification methods to predict if a rookie player will stay over five years. Therefore promote to the professional category.</p>

<a id="intro"></a>
<h2> 2. Introduction </h2>
<p>The National Basket Association (NBA) is one of the most popular and recognized leagues. It is a billion dollars business with millions of viewers around the world. Only in 2018-2019, the combined avenue of teams of the NBA was over 8.7 billion dollars(Nguyen et. al 2021). The main aim of this study is to evaluate the effectiveness of applying Machine Learning (ML) techniques to predict players' future performance, through their primary statistics. To achieve this goal, It will apply basic supervised classification ML methods, such as Dummies Classifier (for establishing a baseline) KNN, Naive Bayes, Logistic Regression, and Random Forrest. The metric score chosen for this project is F2-score. The score elected take after the recomendation published in "Imbalanced Classification with Python" by Jason Brownle, due to have a classification problem with an imbalanced dataset, a positive class more important and false negative more costly.</p>
<p> A sample of 10% of the dataset was taken out for later verification of the predicted models resulting </p> 

<a id="data"></a>
<h2>3.Dataset</h2>
Find the repository in the following link https://data.world/exercises/logistic-regression-exercise-1. The dataset can be split into two types of categories, accumulative variables and percentage variables. Also, it contains the target feature label as (target_5yrs).
<a id="data_clean"></a>
<h3> 3.1 Data Clean</h3>
Given the low number of null data, we decided to drop them, which resulted in the loss of eleven samples. Furthermore, duplicates also represent less than 30 samples so they take out the dataset.
<a id="data_analysis"></a>
<h3> 3.2 Data Analysis</h3>
A diagram is made to visualize the correlation between all the features but also how they interact with the target. 
