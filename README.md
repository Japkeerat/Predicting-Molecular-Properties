# Predicting Molecular Properties

This repository contains my progress and approach towards a data science competition with the same name on Kaggle.

The following table gives a brief description of the files and entries in this table are in the order of attempt I did.

| File | Description | Score | Note to myself | Date Attempted |
| ---- | ----------- | ----- | -------------- | --------------- |
| [Random Forest (untuned)](https://github.com/Japkeerat/Predicting-Molecular-Properties/blob/master/Random_Forest_without_hyperparameter_tuning.ipynb) | A basic Machine learning model with minimal preprocessing and directly applying Random Forest algorithm without any hyperparameter tuning. Main motive was to get my name on the leaderboard first. | 1.177 | At least tune the model next | June 1, 2019 |
| [Random Forest (EDA+untuned)](https://github.com/Japkeerat/Predicting-Molecular-Properties/blob/master/Rnadom_Forest_with_EDA_untuned.ipynb) | Did EDA to find outliers and remove it. Also increased a bit of preprocessing. | 1.174 | When will you tune it? | June 2, 2019 |


Score was calculated with log of mean absolute error which is calculated across all scalar coupling and then averaged across types.

![https://github.com/Japkeerat/Predicting-Molecular-Properties/blob/master/Formula.JPG](https://github.com/Japkeerat/Predicting-Molecular-Properties/blob/master/Formula.JPG)
