# Sales prediction for food items sold at various stores
## Item sales and the features that impact them

**Author**: Shaun van der Merwe


![Alt Text](https://github.com/Shaunnero/Prediction_of_Product-Sales/blob/main/OIP.jpg)



### Business problem:

You are opening a new Store at a particular location. Now, Given the Store Location, Area, Size and other params. Predict the overall revenue/Sale generation of the Store

### Data:
Big Mart Sales Prediction

https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/


## Methods

Regression Metric Selection: Linear regression

Used to predict or explain the relationship between a dependent variable and one or more independent variables.It assumes a linear connection between these variables, represented by a straight line

Regression Metric Selection: Random Forest with GridSearchCV

Random Forest with GridSearchCV is a powerful combination of machine learning techniques used for building predictive models. Random Forest is an ensemble algorithm that combines multiple decision trees to make accurate predictions. GridSearchCV is a method for systematically tuning hyperparameters to find the best configuration for a model


## Results

Linear regresion
Comparing Training vs. Test Performance

The R-squared value for the training data indicates that the model doesnt fit the training data well, capturing 0.67% of the variability.
The R-squared value for the test data indicates that the model generalizes to new, unseen data with an R-squared value of  -8.45%.

In conclusion, our linear regression model demonstrates a very bad performance in predicting the target variable and is Overfitting. Its ability to generalize to new data indicates that it is overly specialized to the training data (overfitting) and too simplistic (underfitting).

Random Forest with GridSearchCV
Comparing Training vs. Test Performance

The R-squared value for the training data indicates that the model doesnt fit the training data well, capturing 69% of the variability.
The R-squared value for the test data indicates that the model generalizes to new, unseen data with an R-squared value of  59%.

In conclusion, this project focused on developing a Random Forest regression model to predict product prices using a range of features. The model's primary objective was to provide accurate estimations for a specific set of attributes. These attributes encompassed crucial factors like Shelf space, Fat Content, Store size, and other pertinent variables, all contributing to the model's predictions. The incorporation of the actual sale price of the product as the target variable allowed the model to discern and approximate the complex interplay between these attributes and the ultimate price.

Our model exhibited promising performance on the training data, demonstrating its capability to fit well and explain a substantial portion of the variance within this dataset. The relatively low values of MAE, MSE, and RMSE, coupled with a favorable R² value of 0.696, underscored its proficiency in capturing the underlying relationships.

However, upon testing the model on unseen data, some nuances emerged. While the test data metrics indicated relatively low MAE and RMSE values, the increased values of MSE and the R² value of 0.596 suggested potential challenges in its generalization to new scenarios. This underscores the importance of refining the model to ensure its robustness across diverse datasets.



#### Visuals
### Insight 1: Overview of the numerical feaures in the data

![Alt Text](https://github.com/Shaunnero/Prediction_of_Product-Sales/blob/main/Screenshot%202023-08-21%20095517.png)


#### Visual 2 Frequency of Fat Content

![Alt Text](https://github.com/Shaunnero/Prediction_of_Product-Sales/blob/main/Screenshot%202023-08-21%20100640.png)

We can observe from the analysis that products labeled as 'low-fat' are more readily available compared to their regular 'full-fat' counterparts. This indicates a noticeable preference for healthier options among consumers, as evidenced by the higher availability of items with reduced fat content

## Model

The final model developed for this project is a Random Forest regression model. This ensemble-based approach combines multiple decision trees to make accurate predictions. Its versatility and ability to handle complex relationships between features make it well-suited for predicting product prices based on various attributes

In summary, the final Random Forest regression model demonstrates favorable performance metrics on both training and test data. Its ability to minimize errors, provide accurate price predictions, and explain a substantial portion of price variability makes it a valuable tool for solving the business problem of predicting product prices. However, there is still room for improvement, especially in enhancing the model's generalization capabilities to unseen data, which can further enhance its real-world applicability.

## Recommendations:

Based on our analysis and model evaluation, we offer the following recommendations:

Feature Importance Analysis: Conduct a comprehensive analysis of feature importance as determined by the Random Forest model. This will help identify which features, such as Shelf space, Fat Content, and Store size, have the most significant impact on predicting product prices. Focus on refining and enhancing these features to potentially improve the model's predictive accuracy.

Further Data Collection: Consider collecting additional data on attributes that could influence product prices but were not included in the current dataset. This could involve gathering more information about factors like brand popularity, packaging design, or promotional strategies. Expanding the dataset in this way may lead to more accurate price predictions.

Model Tuning: Experiment with fine-tuning the hyperparameters of the Random Forest model. Adjust variables such as the number of trees, maximum depth, and minimum samples per leaf, specifically tailored to the context of predicting product prices. Proper tuning can enhance the model's generalization capability and overall performance.

Cross-Validation: Implement k-fold cross-validation to rigorously evaluate the model's performance across different subsets of the data. By assessing the model's consistency and robustness, you can ensure that its predictions remain accurate and reliable.

Ensemble Methods: Explore the potential of ensemble techniques like bagging or boosting, which can improve the model's predictive power by combining multiple models. These techniques could help mitigate any potential overfitting concerns and lead to more reliable predictions.

Collaboration with Domain Experts: Consider collaborating with experts in retail or marketing to gain insights into additional features or nuances that might impact product pricing. Their domain knowledge can guide you in selecting meaningful features and refining the model accordingly.

External Data Integration: Investigate the possibility of integrating external data sources, such as market trends or economic indicators, to enrich your dataset. This broader context could enhance the model's ability to capture pricing variations accurately.

Ongoing Model Evaluation: Continuously monitor and evaluate the model's performance as new sales data becomes available. This iterative process ensures that the model remains up-to-date and effective in providing accurate price predictions.


### For further information

This project was authored by Shaun van der Merwe. You can reach out to me at shaun.vandermerwe@mmltd.co.za.
