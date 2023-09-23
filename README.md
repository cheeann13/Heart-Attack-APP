# A Heart Attack Prediction APP for Clinicians

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://cheeant-heart-attack-app-heart-attack-app-hjks0q.streamlitapp.com/)

# Problem Statement
With just a tiny dataset of 303 entries, can we craft a model that accurately predicts patients at high risk of heart attacks? 
Such a model could be a game-changer, helping doctors intervene earlier and potentially save lives!

## Invalid Inputs in Small Dataset
![image](https://user-images.githubusercontent.com/29735171/180817326-95a4d5d0-358d-4dc4-9fea-af3e5df8941e.png)

It appears that there were errors during data collection, resulting in invalid inputs in 7 of the records. 
Given the dataset's limited size, it's advisable to sidestep imputation to prevent potential distortions in the original data distribution.

## Model Comparison
![model_comparison](https://user-images.githubusercontent.com/29735171/180818231-8a62e42e-c9c3-4ec0-9065-dfb5a2ad3501.jpeg)

Upon evaluation, the combination of Standard Scaler and Logistic Regression yielded the highest accuracy score of 0.85.

## Classification Reports 
![classification_report_0 84](https://user-images.githubusercontent.com/29735171/180818802-d6922a81-f137-4ca9-a0fc-f26bc0c9fac2.png)

Considering the dataset's constraints, the results are commendable! We're now set to transition into the app development phase.

# [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://cheeant-heart-attack-app-heart-attack-app-hjks0q.streamlitapp.com/)

<img width="1422" alt="Screenshot 2022-07-25 at 10 43 30 PM" src="https://user-images.githubusercontent.com/29735171/180819825-d3e5d6a9-4600-4f4c-953c-e2f62f9b25bf.png">
<img width="1427" alt="Screenshot 2022-07-25 at 10 46 57 PM" src="https://user-images.githubusercontent.com/29735171/180819888-8c711c49-0576-4b5d-8585-a63a6f76c486.png">
<img width="1388" alt="Screenshot 2022-07-25 at 10 47 25 PM" src="https://user-images.githubusercontent.com/29735171/180819917-c92d65ab-0e5f-4c83-9fe8-e31bad572f66.png">


## Why Some Mistakes Are Costlier Than The Others? 
Clinicians require robust evidence before integrating new tools into their practice. 
A critical concern raised was the potential ramifications of the app incorrectly classifying high-risk patients as low-risk. 
Such misclassifications could lead to a false sense of security, delaying essential treatments.


## Putting Our Model to Test
A separate dataset, consisting of 10 entries, was provided by clinicians for model validation.

![classification_report_test_data_0 9](https://user-images.githubusercontent.com/29735171/180822362-ebc1f4ba-3163-404e-af9b-f190b0f5e679.png)

## Yeah!
The results were promising! The model's 100% sensitivity in detecting heart attack patients reassured clinicians of its reliability, particularly in minimizing False Negative outcomes.

### Acknowledgments

- Original Dataset: [UCI Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/Heart+Disease)
- Kaggle Dataset: [Kaggle Heart Attack Analysis & Prediction Dataset](https://www.kaggle.com/datasets/rashikrahmanpritom/heart-attack-analysis-prediction-dataset?sort=votes)
