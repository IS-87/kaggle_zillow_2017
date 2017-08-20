# kaggle_zillow_2017
Kaggle Zillow Competition

Data files for this competition can be found on kaggle

Random_Solution.ipynb simply mirrors the existing average error and standard deviation of error.
Predictably, this solution placed me in 3rd spot from the bottom out of 2,200+ entries

Random_Solution_v2.ipynb expands on Random_Solution.ipynb by adding average error of a specific parcelid.
First we figure out if there is a "pull" on error of specific features. Then for every parcelid we record this pull and add all pulls across all columns, before adding this result to our naive solution Random_Solution.ipynb.
In other words, this should in theory be better than Random_Solution.ipynb but I still have no idea what I'm doing.
