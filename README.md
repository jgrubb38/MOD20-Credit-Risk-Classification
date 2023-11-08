# MOD20-Credit-Risk-Classification
Student:  Jennifer Grubb  
Instructor:  Steven Greene  
Bootcamp:  DU-VIRT-DATA-PT-06-2023  
08 November 2023  

## Table of Contents
- [About](#about)
- [Contributing](#contributing)
- [Overview](#overview)
- [Results](#results)
- [Summary](#summary)
  
## About
In this challenge, I used various techniques to train and evaluate a model based on loan risk. I used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.  

## Contributing
N/A  
    
## Overview
The primary purpose of the analysis is to develop a machine learning model to predict loan status (healthy loans vs. high-risk loans) based on financial information and other relevant features. The challenge likely involved identifying loans that may be at higher risk of default or financial instability.  

The main prediction target was the loan status, which is a binary classification task. It involved predicting whether a loan is "0" (healthy) or "1" (high-risk). The analysis aimed to assess the performance of machine learning models in classifying loans into these categories. The value_counts method is used to check the distribution of the loan status (0 and 1) in the dataset, which is essential for understanding class balance or imbalance.

## Results
<b>Machine Learning Model 1:</b>  
<img src="/Images/Model1.png" alt="Model1">  

  * For Label 0 (healthy loan), the logistic regression model performs exceptionally well, with high precision, recall, and F1-score, suggesting that it predicts healthy loans accurately.  
  * For Label 1 (high-risk loan), the logistic regression model performs well, but not as perfectly as it does for Label 0. It has an 86% precision, which means that there are some false positives, and a 91% recall, indicating that it correctly identifies most high-risk loans.  
  * In summary, the logistic regression model performs very well for Label 0 (healthy loans) and reasonably well for Label 1"(high-risk loans). The model is particularly strong at identifying healthy loans with high precision and recall.  

<b>Machine Learning Model 2:</b>  
<img src="/Images/Model2.png" alt="Model2">  

  * For Label 0 (healthy loan), the logistic regression model performs exceptionally well with high precision, recall, and F1-Score, indicating that it predicts healthy loans accurately.  
  * For Label 1 (high-risk loan), the logistic regression model performs well, but not as perfectly as it does for Label 0. It has an 85% precision, indicating that there are some false positives, but it correctly identifies almost all high-risk loans with 99% recall.  
  * In summary, the logistic regression model, fitted with oversampled data, performs very well for Label 0 (healthy loans) and reasonably well for Label 1 (high-risk loans). It excels at predicting healthy loans with high precision and recall, and it also effectively identifies high-risk loans with a high recall score.  

## Summary  
Both models are strong, but there are slight differences in precision and recall for Label 1 (high-risk loans). Machine Learning Model 2 has a higher recall for high-risk loans but a slightly lower precision compared to Model 1. The choice between the two models depends on the problem you are trying to solve and the trade-off between precision and recall. Ultimately, the decision should be based on the specific business requirements and the consequences of false positives and false negatives in your application.  
