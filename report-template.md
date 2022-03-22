# Report: Predict Bike Sharing Demand with AutoGluon Solution
Lisa Hare

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
I actually didn't have any negatives, but if I had I would have had to remove them since there can't be negative bikes.

### What was the top ranked model that performed?
The one with added features

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
I added two additional features by breaking the datetime down into hour and day. These extra features increased the performance.

### How much better did your model preform after adding additional features and why do you think that is?
About 3 points highers. I would guess that the added features helped with accuracy since it was more precise with day and hour.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
It performed worse. I need to read up more on the hyperparameters and play around with them more.

### If you were given more time with this dataset, where do you think you would spend more time?
I would play around with dropping and adding features as well as working more with hyperparameters to optimize Autogluon even more.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score. 

I had trouble adding a table and graphs to the markdown so I also included a notrebook with all of this info in it.
    
### Create a line plot showing the top model score for the three (or more) training runs during the project.

See notebook

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.
See notebook

## Summary
I explored the features and the distribution and then trained a model on it using Autogluon's Tabular prediction. After 10 minutes it reported that the best model was the weighted ensamble L3. The model remained the best even after adding features and tuning hyperparameters. This first score was 1.80. The second score after running it again with two added features of day and hour the score was 4.76. The last score after tuning hyperparameters was .48. This was the lowest so obviously I didn't improve the model with tuning. I believe I could get a better score wikth more time spent understanding the hyperparameters and playing with the various features.