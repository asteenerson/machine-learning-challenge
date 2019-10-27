Of the two completed models I found that random forest was the most successful due to its ability to perform with large amounts of 
features. Since this dataset has 40 different features, I thought random forest would be ideal if I kept them all.  My random 
forest model had an accuracy of 89%. When ranking the importance of the features I found that there weren’t any major factoring 
features as koi_fpflag_ss had the most importance at 10%. 

Of the models I tried, neural network came in second with an accuracy of 85%. I found that due to the predicted values having three possible outcomes, CANDIDATE, CONFIRMED and FALSE POSITIVE I had to one hot the y values. 

I did attempt to tune my hyperparameters, however, I found that even when shaping my data to only five features my laptop was not able to calculate the first set of grid parameters in under an hour. I believe this was because the training data was still 5243 rows and even if reduced to 5 features (5243, 5) I could not get it to calculate in any reasonable amount of time. 
