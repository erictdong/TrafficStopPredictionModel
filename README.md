# TrafficStopPredictionModel
Goal of the project was to investigate if there is any biases (racial, age, gender, etc) in traffic stops and policing.
Using colorado state trooper data, multiple models were created to classify the outcome of a traffic stop given (citation or no citation) given driver information such as race, gender, age, and violation type. 
Models used in clue kNN, Naive Bayes, Logistic Regression, and SVM. Scores were around 72-79 % correct predictions depending on the model, excluding naive bayes.
Initial cleaning of the data showed that ages > 100 were invalid data and dropped columns we weren't interested in. Because there were over 2 million data points, a random 100,000 points were used for our final model and csv. The violations column had over 100000 unique entries, so we took the top 10 violations for our model. 
Future work would include better preprocessing to use all data points and include more violation types. Other target variables could be investigated such as if an arrest was made.
Most interesting note was during preprocessing where hispanics and blacks are twice as likely to get searched and arrested compared to white subjects, despite white subjects representing a large proportion of our data.
