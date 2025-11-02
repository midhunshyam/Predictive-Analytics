# Predictive Analytics: Mutual Funds and ETFs  

This repository contains a machine learning analysis of the [Mutual Funds and ETFs Dataset](https://www.kaggle.com/datasets/stefanoleone992/mutual-funds-and-etfs) from Kaggle.  

Our project focuses on financial data preprocessing, modeling, and imputation to predict and classify fund characteristics. It involves both supervised and unsupervised learning techniques, including neural networks, Bayesian classifiers, and data imputation strategies for handling missing values.

The `PA.ipynb` is main Jupyter Notebook for this project. Contains all methodologies, analysis code, and results in a single, self-contained notebook with detailed information on global mutual funds and exchange-traded funds (ETFs), including financial performance, asset allocation, and fund classifications.


## Machine Learning Methods  

1. **Neural Networks (NN)**  

A feed-forward neural network was designed and trained to predict fund categories. The algorithm learned from historical financial patterns, enabling it to recognise complex, non-linear relationships between variables that simpler models might overlook. This helped improve the accuracy of fund classification and regression tasks.  

2. **Naïve Bayes Classifier**  

A probabilistic model based on Bayes’ theorem was implemented to estimate the likelihood that a fund belonged to a given category. By calculating probabilities from key financial metrics, this approach provided a fast, interpretable baseline for comparison with more advanced machine learning models.  

3. **Support Vector Machine (SVC, RBF Kernel)**  

A Support Vector Classifier using a radial basis function kernel was applied to capture non-linear decision boundaries in the dataset. It effectively separated fund categories by mapping input features into higher-dimensional space, improving precision for complex classification problems.  

4. **Ridge Regression**  

This linear regression method incorporated L2 regularisation to reduce overfitting and stabilise coefficient estimates. It proved useful for modelling relationships between continuous financial indicators while maintaining model interpretability.  

5. **Support Vector Regression (SVR)**  

SVR extended the concept of Support Vector Machines to regression tasks, allowing for flexible prediction of continuous outcomes such as expected returns or volatility. The epsilon-insensitive loss function ensured robustness against small fluctuations in data.  

6. **K-Nearest Neighbours (KNN) Imputation**  

To address missing values, the KNN algorithm was employed to estimate absent data points based on the most similar records in the dataset. This preserved data consistency without introducing significant bias, ensuring high-quality input for model training.  

7. **Cross-Validation and Grid Search**  

Systematic cross-validation was carried out to ensure models generalised well to unseen data. Grid search was then used to tune hyperparameters such as regularisation strength, kernel parameters, and learning rates—optimising model performance.  

8. **Feature Engineering and Scaling**  

All numerical features were standardised using *StandardScaler*, ensuring they contributed equally to the model. Categorical variables were converted into numerical form using one-hot encoding, allowing algorithms to process them efficiently.  

9. **Performance Evaluation**  

Each model was evaluated using appropriate metrics—accuracy, AUC, and confusion matrices for classification tasks, and mean squared error (MSE) and R² for regression. Visual diagnostics such as residual and ROC curves helped interpret and validate model performance.  

10. **Database Schema Design**  

A normalised relational database schema was designed to store mutual fund and ETF data efficiently. This structured foundation supported consistent data retrieval and integration with analytical workflows, ensuring scalability for future research.  

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
