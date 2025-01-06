# Description
This was a binary classification project focused on detecting fraudulent credit card transactions in a highly imbalanced dataset (8.7% fraud cases). I implemented a two-stage undersampling approach combining Tomek Links (to clean decision boundaries) with Random Undersampling (to balance classes). The model prioritized recall to maximize fraud detection while accepting some false positives.

I used a decision tree classifier with randomised hyperparameter search for optimization. The model achieved 99.98% recall while maintaining interpretability. Several feature engineering attempts were explored to capture different fraud patterns, and the optimal combination was discovered empirically using backward feature selection.

# Insights
- Scaling the distribution of features is unnecessary when outliers are contextually meaningful
- Undersampling is suitable for datasets with many samples and (relatively) few features
- Feature engineering can sometimes harm the performance of the model, manually trying feature combinations is inefficient

# Future work
- Consider using probability thresholds to detect more fraudulent transactions
- Consider sorting probabilistic predictions, and then using a bucket purity approach to examine the reliability of the model
- Consider other metrics like F2, which considers both recall and precision, but places greater emphasis on recall
