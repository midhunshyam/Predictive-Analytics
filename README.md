# Predictive Analytics: Mutual Funds and ETFs  

This repository contains a machine learning analysis of the [Mutual Funds and ETFs Dataset](https://www.kaggle.com/datasets/stefanoleone992/mutual-funds-and-etfs) from Kaggle.  

Our project focuses on financial data preprocessing, modeling, and imputation to predict and classify fund characteristics. It involves both supervised and unsupervised learning techniques, including neural networks, Bayesian classifiers, and data imputation strategies for handling missing values.

The `PA.ipynb` is main Jupyter Notebook for this project. Contains all methodologies, analysis code, and results in a single, self-contained notebook with detailed information on global mutual funds and exchange-traded funds (ETFs), including financial performance, asset allocation, and fund classifications.


## Techniques Used  


Neural Networks (NN)
A feed-forward neural network was designed and trained to predict fund categories. The algorithm learned from historical financial patterns, enabling it to recognise complex, non-linear relationships between variables that simpler models might overlook. This helped improve the accuracy of fund classification.

Naïve Bayes Classifier
A probabilistic model based on Bayes’ theorem was implemented to estimate the likelihood that a fund belonged to a given category. By calculating probabilities from the financial metrics, this approach provided a fast, interpretable baseline for comparison with more complex models.

K-Nearest Neighbours (KNN) Imputation
To address missing values within the dataset, the KNN algorithm was applied to estimate absent data points by referencing the most similar records. This preserved the integrity of the dataset without introducing significant bias, ensuring consistent input for subsequent analysis.

Database Schema Design
A normalised relational database schema was created to organise and store mutual fund and ETF data efficiently. This structured foundation supported seamless data retrieval and integration with the analytical models, ensuring scalability and reliability for future financial analyses.


## Individual Contributions  

While the project was a team collaboration, the following tasks were my contributions:

- **End-to-end implementation of Neural Networks (NN)**  
- **Development of the Naive Bayes Classifier**  
- **Complete KNN Imputation pipeline for missing values**  
- **Database schema design and documentation**  


## Key Outcomes

- Successful classification of funds into categories using both NN and Naive Bayes classifiers.
- Efficient imputation of missing financial data using KNN imputation with minimal bias introduction.
- A scalable database schema suitable for storing mutual fund and ETF metadata and financial performance metrics.
