# Week 1 - Introduction

## What is Machine Learning?

`A computer program is said to learn from experience E with respect to some class of tasks T and performance measure P, if its performance at tasks in T, as measured by P, improves with experince E.`

Example: playing checkers.

E = the experience of playing many games of checkers
T = the task of playing checkers
P = the probability that the program will win the next game

Any machine learning problem can be assigned to one of two broad classifications:
- Supervised learning and Unsupervised learning

`Regression: Predict continous value output(price)`

You can check if a function is continuous check the following:
1) does f(c) exists?
2) does limit f(x) exists?
         x->c
3) does the limit f(x)=f(c) exists?
             x->c
Then function is contious at the point.


## Supervised learning
In supervised learning, we are given a data set and already know what our correct output should look like, having the idea that there is a relationship between the input and the output.

Categorized as:
1) Regression -> We are trying to predict results within a continuous output, meaning that we are trying to map input variables to some continuous funtion.
```
Example 1: Given data about the size of the houses on the real estate market, try to predict their price. Price as a function of size is a continuous output, so this is a regression problem.

Example 2: Given a picture of a person, we have to predict their age on the basis of the given picture
```
2) Classification -> We are instead trying to predict results in a discrete(0 or 1) output, meaning that we trying to input variables into discrete categories.
```
Example 1: Given data about the size of the houses on the real estate market, try to classify if the house "sells for more or less than the asking price". Here we are classifying the houses based on price into two discrete categories.

Example 2: Given a patient with a tumor, we have to predict whether the tumor is malignant or benign.
```

## Unsupervised learning
Unsupervised learning allows us to approach problems with little or no idea what our results should look like. We can derive structure from data where we don't necessarily know the effect of the variables.

We can derive this structure by clustering the data based on relationships among the variables in the data. With unsupervised learning there is no feedback based on the prediction results.

Example:

Clustering: Take a collection of 1,000,000 different genes, and find a way to automatically group these genes into groups that are somehow similar or related by different variables, such as lifespan, location, roles, and so on.

Non-clustering: The "Cocktail Party Algorithm", allows you to find structure in a chaotic environment. (i.e. identifying individual voices and music from a mesh of sounds at a cocktail party).

## Model Representation

x^(i) denoted the "input" variable, also called input features and y^(i) denotes the "output" or target variable that we are trying to predict (price). A pair (x^(i), y^(i)) is called a training example. m is called a training set.

Given a training set, to learn a function h: X -> Y so that h(x) is a good predictor for the corresponding value of y. h is called a hypothesis

![Model Representation](https://github.com/graciasrochelle/Machine-Learning/blob/week1/image1.png)

When the target variable that we're trying to predict is continous, such as the housing example, we call the learning problem a regression problem. When y can take on only a small number of discrete values (such as if, given the living area, we predict if a dwelling is a house or an apartment) we call it a classification problem.

## Cost function
Otherwise called the "Squared error function", or "Mean squared error". This takes an average difference of all the results of the hypothesis with inputs from x's and the actual output y's.

The goalis to try to minimize the cost function.

## Linear Regression with one variable - Gradient Descent


## Matrices and Vectors
Matrices rectangular array of numbers. 2D array. Denoted by upper case alphabets.
Dimention of matrix: Number of rows X Number of columns

Vector: An n * 1 matrix. 4D vector. 1-indexed vs 2-indexed. Denoted by lower case alphabets.

Prediction = Data Matrix * Parameters

[m * n] * [n * o] = m * o

Matrices that don't have an inverse are "singular" or "degenerate"
