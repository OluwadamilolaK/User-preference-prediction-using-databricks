# User-preference-prediction-using-databricks
# Overview
In this project, the aim is to explore and analyse a dataset extracted from Steam, named steam-200k.csv, which contains details of games purchased and played by users along with the corresponding behavior and playtime. The dataset consists of four columns:
•	A unique identifier for each member 
•	The name of the game they purchased or played 
•	Details of the member behaviour, either ‘purchase’ or ‘play’. Because a game has to be purchased before it can be played, hence, there will be two entries for the same game/member combination in some instances 
•	This column is set to 1 for rows where the behavior is ‘purchase’. For rows where the behavior is ‘play’ the value in the fourth column corresponds to the number of hours of play 

The objective is to utilize this dataset to build a collaborative filtering recommender system using Apache Spark's MLlib. Collaborative filtering is a popular technique for making personalized recommendations by analyzing user behavior and similarities between users or items. By training a collaborative filtering model on the provided data, we aim to generate accurate recommendations for users based on their purchase and play behavior. By leveraging the power of collaborative filtering and Apache Spark's MLlib, we aim to provide valuable recommendations to Steam users, enhancing their gaming experience and driving engagement on the platform.
# EDA
Visualization was done particularly displaying the purchase and play feature with other features.
# Data Preparation
We will preprocess the data to prepare it for training the recommender system. This may involve converting the data into the required format, splitting it into training and test sets, and generating unique integer IDs for the games. Model evaluation and hyperparameter is then performed on the data.

# Conclusion
A lower RMSE indicates better performance, so an RMSE of 0.0774 suggests that the model's predictions are, on average, approximately 0.0774 units away from the actual values. This value could be considered satisfactory depending on the context of your specific problem and the range of the target variable.
Summarily, the tuned ALS model with a rank of 5 and a regularization parameter of 0.01 performs well based on the relatively low RMSE of 0.0774 on the test data. The high level of accuracy shows that the model can accurately predict user preferences or behaviors because its predictions are typically close to the actual values. 

# Recommendation
When the ALS model's hyperparameters are tuned to achieve a low RMSE, it shows that the model is doing a good job of predicting user preferences. By providing specific and relevant recommendations, this precise recommendation system can increase user satisfaction and engagement in real-world applications.

When a platform recognizes its users' preferences and recommends content or products that suit their interests, users are more likely to interact with it. You can provide users with a more customized experience by utilizing the tuned ALS model, which could result in higher conversion rates, longer user retention periods, and happier users.

Furthermore, a precise recommendation system can support other corporate goals like raising revenue, boosting metrics for user engagement, and improving the user experience in general. As a result, implementing the tuned ALS model in practical applications could greatly benefit your platform or company.


