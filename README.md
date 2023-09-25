# Credit Card Transactions Fraud Analysis and Modeling: How to deal with Imbalanced data and why 99% precision is not always good.

<img height="550em" src="https://blog.saginfotech.com/wp-content/uploads/2019/04/credit-card-frauds.jpg" alt="hi" class="inline"/>

> In today's increasingly digital world, the use of credit cards for online and offline transactions has become an integral part of our daily lives. While this convenience offers numerous advantages, it also opens the door to a growing threat - credit card fraud. To combat this menace, the field of machine learning has emerged as a powerful ally, enabling us to develop robust fraud detection systems capable of safeguarding our financial transactions.

Credit card fraud detection is a critical application of machine learning, as it directly impacts individuals, businesses, and financial institutions worldwide. However, it's no simple task. The inherent imbalance in credit card transaction data, where legitimate transactions vastly outnumber fraudulent ones, poses a significant hurdle. That happens because traditional machine learning models may struggle to perform on such imbalanced dataset (an imbalanced dataset means that the event we want to predict is rare). This causes the model to struggle to recognize patterns in fraud transactions, and can result in poor predictions.

In this project, we'll analyze data from credit card transactions and create a model that is able to surpass this obstacle and recognize patterns from fraud transactions and be able to predict 89% of all subsequent frauds.

We'll guide you through the following key steps:

1. **Exploratory Data Analysis and Preprocessing:** We'll start by exploring the dataset with univariate and multivariate analysis, to better understand our data and extract valuable insights of which information we can use to help us recognize frauds and which columns we'll need to transform to be able to use in our model, aswell as addressing issues such as missing data and outliers.

2. **Feature Engineering:** Here we'll demonstrate how to extract meaningful features from the transaction data and create a robust feature set for our models. In machine learning, handling categorical columns often necessitates translating information into numeric format. For instance, instead of using a column with "Yes" or "No" values, we convert them to "1" or "0," allowing the models to perform mathematical operations effectively. This process is called categorical data encoding, and is a very important part of all machine learning models, since we pretty much always will have categorical information, and we cannot afford to not use it, because they are valuable!

3. **Imbalanced Data Handling:** In this module we'll cover a technique called undersampling, which is basically consists in reducing the numbers of non-events (in this case normal transactions) in our dataset. This will reduce the rarity of the fraud events in our dataset and will help our model to better identify patterns that can help us to detect frauds.

4. **Feature Importance:** Here we'll choose which feature (columns) to use in our model, by evaluating their predictive power and setting them importances numbers, which will help us to choose the information that will enter the machine learning models.

5. **Setting up:** After selecting the columns we'll use in our models, we need to split our data in 3 parts: Training, validation and test. The training set will be used to train the models, the validation dataset will be used to checking the quality of the models and optimize the parameters of it, while the test data will be use to evaluate the final results of the model. Splitting the dataset is a very important concept in machine learning, as it allows us to evaluate our models on unbiased data. If we train our model and evaluate the results in the same dataset, the model can memorize the results instead of identify the real patterns, and consequently fail to predict the outputs for other data. This phenomenon is called overfitting.

6. **Training the Model:** We'll use all the features we selected in the previous topic to train our machine learning models and select the models performs better in our dataset.

7. **Tuning the Hyperparameters:** In this section, we will enhance our model's performance by fine-tuning its hyperparameters using Bayesian optimization. Bayesian Optimization is a method that follows a structured approach grounded in Bayes' Theorem. It guides the search for optimal settings in a way that is both efficient and highly effective for solving complex optimization challenges.

8. **Results evaluation and Conclusion:** Here we finish our work by evaluating the results and discussing the main metrics of the model.
