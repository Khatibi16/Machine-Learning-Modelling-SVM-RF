# Machine-Learning-Modelling-SVM-RF

This project tackles a binary classification problem using a dataset with 1,400 samples and 20 numerical features. The objective was to explore and compare the performance of two machine learning algorithms: Support Vector Machine (SVM) and Random Forest (RF).

The process began with exploratory data analysis (EDA) to understand feature distributions, detect outliers, and examine correlations. Most features were approximately normally distributed, and no significant multicollinearity was observed. Outliers were present but retained, with standardization applied to mitigate their impact—especially for SVM, which is sensitive to extreme values.

Initial baseline models were trained using default hyperparameters. The SVM achieved an accuracy of 81%, while the Random Forest model performed better with 84% accuracy. Both models were then optimized using Grid Search and Randomized SearchCV. While SVM performance remained stable, the Random Forest model improved significantly, achieving a final accuracy of 86.78% and an AUC-ROC of 0.926, outperforming SVM across all key metrics including precision, recall, and F1-score.

The final model selected was the Random Forest Classifier, fine-tuned with optimized parameters and retrained on the full dataset. It was then used to generate predictions on a test set, with results saved to test_predictions.txt. Overall, the project demonstrates a complete ML pipeline—from data analysis to model tuning and deployment—highlighting Random Forest as the superior choice for this classification task.
