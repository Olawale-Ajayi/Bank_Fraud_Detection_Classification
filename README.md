# Bank_Fraud_Detection_Classification

This is a classification Task that use various Machine Learning algorithm to determine fraudulent Transaction in a Bank Datasets.<br>
The Datasets comprises of over 200000 line items with two targets: Non Fraud and Fraud which are labeled encoded.<br>
An extra care is taked to avoid data leakage when removing outliers in the datasets. The zscore for the removal is set at 11 to retain more datasets in the lower class target (Non Fraud)<br>
The Non Fraudlent transaction covers over 99% of the targets creating and inbalance problem in the data<br>
Random sampling technique like Undersamling and Oversampling are used to balance the datasets<b>
5 differents classfication algorithms are implemented on the Undersapmpled and Oversampled datsets, cross validating the accuracy of each model. <br>

# In Summary

5 different algorithms run are:
1. Support Vector machine
2. Logistic Regression
3. Decision Tree
4. Random Forest
5. KNearest Neighbors

Each algorithms runs through 5 folds of the training set using StrarifiedKfold in skleran. These folds are cross validated to get their validation score on each fold
on the validation set<br>

The Logistic regression outperformed other algorithm reaching over 92% for the Undersampled data and over 93% for the oversampled data on the validation sets<br>
The precision recall curve  and roc chart are plotted for both the undersampled model and Oversampled model.<br>
The Oversampled  data return more True positive than False Negative than the Undersampled data which is what is desired for such an imbalanced data



Overall, The Algorithm performs very well on the test set with over 93% accuracy
This shows that the algorithm will be able to detect more Fraudulent Transaction (True Positive) than Misclassify them as False positive (Non Fraud)









