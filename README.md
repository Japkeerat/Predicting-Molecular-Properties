# Predicting Molecular Properties

This repository contains my progress and approach towards a data science competition with the same name on Kaggle. Download the dataset from [here](https://www.kaggle.com/c/champs-scalar-coupling/data) (Signup required)

The following table gives a brief description of the files and entries in this table are in the order of attempt I did. Point to note is that, during the first three attempts, incomplete data set was taken. The Structures file was never used.

| File | Description | Score | Note to myself | Date Attempted |
| ---- | ----------- | ----- | -------------- | --------------- |
| [Random Forest (untuned)](https://github.com/Japkeerat/Predicting-Molecular-Properties/blob/master/Random_Forest_without_hyperparameter_tuning.ipynb) | A basic Machine learning model with minimal preprocessing and directly applying Random Forest algorithm without any hyperparameter tuning. Main motive was to get my name on the leaderboard first. | 1.177 | At least tune the model next | June 1, 2019 |
| [Random Forest (EDA+untuned)](https://github.com/Japkeerat/Predicting-Molecular-Properties/blob/master/Rnadom_Forest_with_EDA_untuned.ipynb) | Did EDA to find outliers and remove it. Also increased a bit of preprocessing. | 1.174 | When will you tune it? | June 2, 2019 |
| [Random Forest (Semituned)](https://github.com/Japkeerat/Predicting-Molecular-Properties/blob/master/Random_Forest_Tuned.ipynb) | Only tuned number of estimators and oob_score for now. Just wanted to see how much impact this can make on the score. This took around 7.5 hours. And still no improvement in score. | 1.174 | Don't spend time tuning it. Change algorithm. | June 3, 2019 |
| [XGBoost (untuned)](https://github.com/Japkeerat/Predicting-Molecular-Properties/blob/master/xgboost_untuned.ipynb) | An XGBoost model with default parameters. This time, all of the dataset was used and preprocessed. | 1.226 | From next time on, use GPU for training XGBoost. Also change algorithm. | June 5, 2019 |
| [LightGBM-1](https://github.com/Japkeerat/Predicting-Molecular-Properties/blob/master/LightGBM_version1.ipynb) | A LightGBM model with some tuning and using all dataset. Also adding one more column 'distance' as other kagglers noted its importance. | 0.527 | Go on to tune it in better way | June 6, 2019 |
| [Extra Trees (Untuned)](https://github.com/Japkeerat/Predicting-Molecular-Properties/blob/master/Extra%20Trees%20Untuned.ipynb) | A basic model with many derived features from other files that had no meaning yet in the test set. Main reason is that I had just read about this approach and wanted to try with an algorithm I never really worked with before. | 0.231 | Tune it as well. | June 8, 2019 |
| [LightGBM-2](https://github.com/Japkeerat/Predicting-Molecular-Properties/blob/master/LightGBM_Extra_Features.ipynb) | A LightGBM model that uses some derived features from distance between atoms and effects for a particular molecule. Tuned it up a bit as well. | -0.120 | Next check the score without external data. | June 15, 2019 |

Score was calculated with log of mean absolute error which is calculated across all scalar coupling and then averaged across types.

![https://github.com/Japkeerat/Predicting-Molecular-Properties/blob/master/Formula.JPG](https://github.com/Japkeerat/Predicting-Molecular-Properties/blob/master/Formula.JPG)

External data usage details:

| Dataset link | Used in |
| ------------ | -------- |
| [Simple Molecular Geometry Features](https://www.kaggle.com/bigironsphere/simple-molecular-geometry-features) | [LightGBM-2](https://github.com/Japkeerat/Predicting-Molecular-Properties/blob/master/LightGBM_Extra_Features.ipynb) |
