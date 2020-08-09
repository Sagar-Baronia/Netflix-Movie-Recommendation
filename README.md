# ***Netflix Movie Recommendation***

### ***Challenge Description***

*__Netflix__ is all about connecting people to the movies they love. To help customers find those movies, they developed world-class movie recommendation system: __CinematchSM__. Its job is to predict whether someone will enjoy a movie based on how much they liked or disliked other movies. Netflix use those predictions to make personal movie recommendations based on each customer’s unique tastes. And while Cinematch is doing pretty well, it can always be made better.*

*Now there are a lot of interesting alternative approaches to how Cinematch works that netflix haven’t tried. Some are described in the literature, some aren’t. We’re curious whether any of these can beat Cinematch by making better predictions. Because, frankly, if there is a much better approach it could make a big difference to our customers and our business.*

*__Credits:__ https://www.netflixprize.com/rules.html*

*Netflix provided a lot of anonymous __rating data__, and a __prediction accuracy__ bar that is __10%__ better than what Cinematch can do on the same training data set. Accuracy is a measurement of how closely predicted ratings of movies match subsequent actual ratings.*

### ***Real World Business Objectives and Constraints***

***Objectives :***



1.   *Predict the rating that a user would give to a movie that he ahs not yet rated.*
2.   *Minimize the difference between predicted and actual rating i.e.RMSE and MAPE.*

***Constraints :***

1.   *Some form of interpretability.*

## ***Machine Learning Problem Statement***

### ***Data Overview***

*__Data Source :__*

*Get the data from : https://www.kaggle.com/netflix-inc/netflix-prize-data/data*

*__Data files :__*

*combined_data_1.txt*
*combined_data_2.txt*
*combined_data_3.txt*
*combined_data_4.txt*
*movie_titles.csv*
  
*The first line of each file [combined_data_1.txt, combined_data_2.txt, combined_data_3.txt, combined_data_4.txt] contains the movie id followed by a colon. Each subsequent line in the file corresponds to a rating from a customer and its date in the following Sequence : CustomerID, Rating, Date*

*__Data Ranges :__*

*MovieIDs range from 1 to 17770 sequentially.*
*CustomerIDs range from 1 to 2649429, with gaps. There are 480189 users.*
*Ratings are on a five star (integral) scale from 1 to 5.*
*Dates have the format YYYY-MM-DD.*

## ***Mapping the real world problem to a Machine Learning Problem***

*__Type of Machine Learning Problem :__*

*For a given movie and user we need to predict the rating would be given by the user to the movie. The given problem is a Recommendation problem. It can also seen as a Regression problem*

*__Performance metric :__*

*   *Mean Absolute Percentage Error*
*   *Root Mean Square Error*

*__Machine Learning Objective and Constraints :__*

*   *Minimize RMSE.*
*   *Try to provide some interpretability.*
