# kaggle_zillow_2017
Kaggle Zillow Competition

Data files for this competition can be found on kaggle

Random_Solution.ipynb simply mirrors the existing average error and standard deviation of error.
Predictably, this solution placed me in 3rd spot from the bottom out of 2,200+ entries (Score 0.1530912)

Random_Solution_v2.ipynb expands on Random_Solution.ipynb by adding average error of a specific parcelid.
First we figure out if there is a "pull" on error of specific features. Then for every parcelid we record this pull and add all pulls across all columns, before adding this result to our naive solution Random_Solution.ipynb.
In other words, this should in theory be better than Random_Solution.ipynb but I still have no idea what I'm doing.
Turns out this one is really, really poor (Score 0.6675998)

Random_Solution_v3.ipynb is the simplest "solution". It sets all the predictions to the current mean of logerror in the training set.
Score is 0.0651279.

Random_Solution_v4.ipynb is a combination of Random_Solution_v3.ipynb with the specific feature "pull" of Random_Solution_v2.ipynb. Score 0.0652980.

Random_Solution_v6.ipynb attempts to fix Random_Solution_v2.ipynb. The score of 0.6675998 didn't make sense. Where duplicate sales were made during the year, only first record was kept. Score is 0.0651220.

Random_Solution_v6.ipynb attempts to fix Random_Solution_v2.ipynb. The score of 0.6675998 didn't make sense. Where duplicate sales were made during the year, only last record was kept. Score is 0.0651226.
