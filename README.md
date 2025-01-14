# Introduction to Machine Learning 

## Table of Contents
1. [Introduction](#introduction)
2. [Machine Learning vs Programming](#machine-learning-vs-programming)
3. [Types of Machine Learning](#types-of-machine-learning)
    - [Supervised Learning](#supervised-learning)
    - [Unsupervised Learning](#unsupervised-learning)
    - [Semi-Supervised Learning](#semi-supervised-learning)
    - [Reinforcement Learning](#reinforcement-learning)
4. [Applications of Machine Learning](#applications-of-machine-learning)
5. [Evolution of Machine Learning](#evolution-of-machine-learning)
    - [Past](#past)
      - [Rule-Based Systems (1950s-1960s)](#rule-based-systems-1950s-1960s)
      - [First AI Winter (1970s-1980s)](#first-ai-winter-1970s-1980s)
      - [Expert Systems (1980s)](#expert-systems-1980s)
      - [Statistical Methods (1990s)](#statistical-methods-1990s)
    - [Present](#present)
      - [Rise of Neural Networks (2010s-Now)](#rise-of-neural-networks-2010s-now)
      - [Big Data and Computational Power](#big-data-and-computational-power)
      - [Diverse Applications](#diverse-applications)
      - [Personalization and Recommendation Systems](#personalization-and-recommendation-systems)
      - [Transfer Learning and Pre-trained Models](#transfer-learning-and-pre-trained-models)
    - [Future](#future)
      - [Advancements in Neural Architectures](#advancements-in-neural-architectures)
      - [Explainability and Trust](#explainability-and-trust)
      - [Interdisciplinary Collaboration](#interdisciplinary-collaboration)
      - [Edge Computing and ML](#edge-computing-and-ml)
      - [AI Beyond Silicon](#ai-beyond-silicon)
      - [Continued Focus on Responsible AI](#continued-focus-on-responsible-ai)
      - [Human-Augmented AI](#human-augmented-ai)
      - [Enhanced Transfer Learning](#enhanced-transfer-learning)
6. [Data Preprocessing](#data-preprocessing)
    - [Checking Data Types and Values](#checking-data-types-and-values)
    - [Data Cleaning](/data-cleaning.ipynb)
    - [Data Transformation](#data-transformation)
    - [Data Reduction](#data-reduction)
    - [Label Encoding](#label-encoding)
    - [Identifying Data Distribution](#identifying-data-distribution)
    - [Statistical Values](#statistical-values)
    - [Plotting Data](#plotting-data)
    - [Steps in Data Preprocessing](#steps-in-data-preprocessing)
    - [Data Loading](#data-loading)
    - [Handling Missing Values](#handling-missing-values)
    - [Standardization](#standardization)
    - [Visualization](#visualization)
    - [Handling Categorical Variables](#handling-categorical-variables)
    - [Feature Selection](#feature-selection)
    - [Feature Scaling](#feature-scaling)
    - [Dimensionality Reduction](#dimensionality-reduction)
    - [Feature Encoding](#feature-encoding)
    - [Statistical Analysis](#statistical-analysis)
    - [Data Types](#data-types)
      - [Categorical](#categorical)
      - [Numerical](#numerical)
      - [Ratio Scale](#ratio-scale)
      - [Interval](#interval)
      - [Ordinal](#ordinal)
      - [Nominal](#nominal)
      - [Time](#time)
      - [Count](#count)
    - [Inconsistent Values](#inconsistent-values)
    - [Duplicate Values](#duplicate-values)
    - [Outliers](#outliers)
    - [Anomaly Detection](#anomaly-detection)
7. [Terminology: Feature Vectors](#terminology-feature-vectors)
8. [Multi-Dimensional Feature Space](#multi-dimensional-feature-space)
9. [Iris Dataset](#iris-dataset)
10. [Basic Terminology](#basic-terminology)
11. [Roadmap for Building ML Systems](#roadmap-for-building-ml-systems)
12. [What is Data Science?](#what-is-data-science)
13. [What is Data Mining?](#what-is-data-mining)
14. [What is Machine Learning?](#what-is-machine-learning)
15. [Preparation of Environment](#preparation-of-environment)
    - [Installation of Anaconda, Jupyter Notebook, and PyCharm](#install)
    - [Introduction to Jupyter Notebook](/intro.ipynb)
16. [Installation of Scikit Learn](#installation-of-scikit-learn)
    - [Regression and Iris Dataset](#regression-and-iris-dataset)
17. [Iris Data for Beginners](/iris-data-for-beginners.ipynb)
18. [Notations](#notations)
19. [Regression](#regression)
    - [Linear Regression](#linear-regression)
20. [Cost Function](#cost-function)
    - [Sum of Squared Error (SSE)](#sum-of-squared-error-sse)
21. [Straight-Line Equation](#straight-line-equation)
22. [Best Fit Prediction Line](#best-fit-prediction-line)
23. [Multiple Linear Regression](#multiple-linear-regression)
    - [Gradient Descent](#gradient-descent)
24. [Gradient Descent Algorithm](#gradient-descent-algorithm)
25. [House Price Data](#house-price-data)
26. [Prediction Error](#prediction-error)
27. [Cost Function (SSE)](#cost-function-sse)
    - [Mean Squared Error](#mean-squared-error)
28. [Standardized Data](#standardized-data)
29. [Min-Max Standardization](#min-max-standardization)
30. [Steps in Gradient Descent](#steps-in-gradient-descent)
    - [Initialize Weights](#initialize-weights)
    - [Calculate Gradients](#calculate-gradients)
    - [Adjust Weights](#adjust-weights)
    - [Calculate New Weights](#calculate-new-weights)
    - [Repeat Process](#repeat-process)
31. [Partial Derivatives](#partial-derivatives)
32. [Learning Rate](#learning-rate)
    - [Support Vector Machine (SVM)](#support-vector-machine-svm)
33. [Support Vector Machine (SVM)](#support-vector-machine-svm)
34. [Key Concepts](#key-concepts)
    - [Support Vectors](#support-vectors)
    - [Hyperplanes](#hyperplanes)
    - [Marginal Distance](#marginal-distance)
    - [Linear Separable Points](#linear-separable-points)
    - [Nonlinear Separable Points](#nonlinear-separable-points)
35. [Splitting the Data](#splitting-the-data)
36. [Basic Idea of SVM](#basic-idea-of-svm)
37. [Important Concepts in SVM](#important-concepts-in-svm)
    - [Support Vectors](#support-vectors)
    - [Hyperplane](#hyperplane)
    - [Margin](#margin)
38. [Regularization](#regularization)
    - [C Parameter](#c-parameter)
39. [Kernels](#kernels)
    - [Linear Kernel](#linear-kernel)
    - [Non-Linear Kernel](#non-linear-kernel)
    - [Radial Basis Function (RBF)](#radial-basis-function-rbf)
    - [Sigmoid](#sigmoid)
    - [Polynomial](#polynomial)
    - [Exponential](#exponential)
40. [Kernel Trick](#kernel-trick)
41. [Pros of SVM](#pros-of-svm)
42. [Cons of SVM](#cons-of-svm)
43. [Applications of SVM](#applications-of-svm)
44. [Predictive Modeling](#predictive-modeling)
    - [Artificial Neural Networks (ANN)](#artificial-neural-networks-ann)
45. [Artificial Neural Networks (ANN)](#artificial-neural-networks-ann)
46. [Biology and Neural Networks](#biology-and-neural-networks)
    - [McCullock-Pitts (MCP) Neuron](#mccullock-pitts-mcp-neuron)
47. [Perceptron Rule](#perceptron-rule)
48. [Simple Example of a Perceptron](#simple-example-of-a-perceptron)
49. [Binary Classification Example](#binary-classification-example)
50. [Perceptron Learning Rule of Rosenblatt](#perceptron-learning-rule-of-rosenblatt)
    - [Steps of the Perceptron Rule](#steps-of-the-perceptron-rule)
51. [Update Rule Example](#update-rule-example)
52. [Linearly and Non-Linearly Separable Data](#linearly-and-non-linearly-separable-data)
53. [Iris Database Example](#iris-database-example)
54. [Python Implementation](#python-implementation)
    - [K-Nearest Neighbors (KNN), Decision Tree, Random Forest, and Clustering](#k-nearest-neighbors-knn-decision-tree-random-forest-and-clustering)
55. [K-Nearest Neighbors (KNN) Algorithm](#k-nearest-neighbors-knn-algorithm)
    - [Steps in KNN](#steps-in-knn)
    - [Normalization and Standardization in KNN](#normalization-and-standardization-in-knn)
    - [Distance Metrics in KNN](#distance-metrics-in-knn)
56. [KNN Algorithm Examples](#knn-algorithm-examples)
57. [Choosing the Factor 'k' in KNN](#choosing-the-factor-k-in-knn)
58. [Decision Tree Learning](#decision-tree-learning)
    - [Decision Tree Structure](#decision-tree-structure)
59. [Decision Tree Node Splitting](#decision-tree-node-splitting)
    - [Information Gain (IG)](#information-gain-ig)
    - [Entropy](#entropy)
    - [Gini Index](#gini-index)
60. [Advantages of Decision Trees](#advantages-of-decision-trees)
61. [Disadvantages of Decision Trees](#disadvantages-of-decision-trees)
62. [Random Forests](#random-forests)
    - [Steps in Random Forest](#steps-in-random-forest)
63. [Advantages of Random Forests](#advantages-of-random-forests)
64. [Hyperparameters in Random Forests](#hyperparameters-in-random-forests)
65. [Random Forest Implementation with Python Codes](#random-forest-implementation-with-python-codes)
66. [Feature Selection](#feature-selection)
    - [Sequential Backward Selection (SBS)](#sequential-backward-selection-sbs)
67. [Feature Importance with Random Forests](#feature-importance-with-random-forests)
68. [Performance Evaluation Metrics](#performance-evaluation-metrics)
69. [Unsupervised Learning](#unsupervised-learning)
70. [Clustering](#clustering)
    - [K-Means Algorithm](#k-means-algorithm)
71. [Elbow Method for Optimal Number of Clusters](#elbow-method-for-optimal-number-of-clusters)
72. [Finding Cluster Centers](#finding-cluster-centers)
73. [Hierarchical Clustering](#hierarchical-clustering)
    - [Agglomerative Hierarchical Clustering](#agglomerative-hierarchical-clustering)
74. [Dimensionality Reduction](#dimensionality-reduction)
    - [Feature Selection vs Feature Extraction](#feature-selection-vs-feature-extraction)
75. [Logistic Regression](#logistic-regression)
    - [Logit Function](#logit-function)
    - [Sigmoid Function](#sigmoid-function)
    - [Linear Regression vs Logistic Regression](#linear-regression-vs-logistic-regression)
76. [Logistic Regression vs SVM](#logistic-regression-vs-svm)
77. [Overfitting](#overfitting)
    - [High Variance](#high-variance)
    - [Underfitting (High Bias)](#underfitting-high-bias)
78. [Avoiding Overfitting](#avoiding-overfitting)
    - [Reducing Number of Features](#reducing-number-of-features)
    - [Regularization](#regularization)
79. [Regularization Penalty Terms](#regularization-penalty-terms)
80. [L1 and L2 Regularization](#l1-and-l2-regularization)
    - [LASSO](#lasso)
    - [Ridge Regression](#ridge-regression)
