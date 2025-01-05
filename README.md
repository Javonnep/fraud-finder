# Description
This was a binary class classification project. The target feature was fraudulent, referring to credit transactions. I used undersampling to balance the dataset and recall to ensure that I prioritised detecting as many fraudulent transactions as possible. I used a random forest classifier in part because ensemble methods are very powerful, and also because they remove the need for feature scaling. My final recall on an unseen validation dataset was a perfect 1.0.

# Insights
- Scaling the distribution of features is unnecessary when outliers are contextually meaningful
- Undersampling is suitable for datasets with many samples and (relatively) few features
- Feature engineering can sometimes harm the performance of the model

# Future work
- Consider using probability thresholds to detect more fraudulent transactions
