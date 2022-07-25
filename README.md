# A Heart Attack Prediction APP for Clinician

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://cheeant-heart-attack-app-heart-attack-app-hjks0q.streamlitapp.com/)

# Problem Statement
Given a very small datasets (303 entries), could we build and train a good enough model that predicts patient with high risk of getting a heart attack, and aids clinicians in providing earlier intervention? 

# Dataset
![image](https://user-images.githubusercontent.com/29735171/180815789-b81a07b4-1b70-4e33-8908-e6e68a36e04a.png)
![image](https://user-images.githubusercontent.com/29735171/180823958-30e0622d-74c2-4e98-910b-da6ae3d3df85.png)

Lucky for us, this is a almost a balance datasets, oversampling is not needed. 

# Data Cleaning
![image](https://user-images.githubusercontent.com/29735171/180817326-95a4d5d0-358d-4dc4-9fea-af3e5df8941e.png)

Ooops! Somebody made a mistake while collecting data, and we have some invalid inputs in 7 of the entries.

Since this is a very small dataset, it is better to avoid the imputation as it mights skew our data from it's original distribution.

# Model Comparison
![model_comparison](https://user-images.githubusercontent.com/29735171/180818231-8a62e42e-c9c3-4ec0-9065-dfb5a2ad3501.jpeg)

Standard Scaler and Logistic Regression gives us the highest accuracy score, at 0.85.

## Classification Reports 
![classification_report_0 84](https://user-images.githubusercontent.com/29735171/180818802-d6922a81-f137-4ca9-a0fc-f26bc0c9fac2.png)

It's not too bad with the limited dataset! We are ready to build an app.

# [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://cheeant-heart-attack-app-heart-attack-app-hjks0q.streamlitapp.com/)

<img width="1422" alt="Screenshot 2022-07-25 at 10 43 30 PM" src="https://user-images.githubusercontent.com/29735171/180819825-d3e5d6a9-4600-4f4c-953c-e2f62f9b25bf.png">
<img width="1427" alt="Screenshot 2022-07-25 at 10 46 57 PM" src="https://user-images.githubusercontent.com/29735171/180819888-8c711c49-0576-4b5d-8585-a63a6f76c486.png">
<img width="1388" alt="Screenshot 2022-07-25 at 10 47 25 PM" src="https://user-images.githubusercontent.com/29735171/180819917-c92d65ab-0e5f-4c83-9fe8-e31bad572f66.png">

# Why Some Mistakes Are More Costly Than The Others? 
Clinicians are not that easily convinced, they need more proofs before they could use our app for references.
They also raised an important point that, it would be catastrophic if our app falsely mark high risk patient as no risk, giving both parties a false sense of security and no treatment is given to the patient untill it is too late.

# Performance Evaluation
They sent a completely new dataset of 10 entries, for model evaluation.

![classification_report_test_data_0 9](https://user-images.githubusercontent.com/29735171/180822362-ebc1f4ba-3163-404e-af9b-f190b0f5e679.png)

## Our model nails it!
More importantnly, the 100% of sensitivity on heart attack patient has just proves the clinicians that this model is good in predicting the True Positive class. The can now sleep soundly knowing that this model would not give them a lot of False Negative results. 

# Credits
The origin: https://archive.ics.uci.edu/ml/datasets/Heart+Disease

Clean dataset: https://www.kaggle.com/datasets/rashikrahmanpritom/heart-attack-analysis-prediction-dataset?sort=votes



