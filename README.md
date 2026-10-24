# SWYNEX-Machine-Learning-Model
Machine Learning Model Training and Evaluation
Machine Learning Models

1. Logistic Regression

Logistic Regression is used as a baseline classification model. It works well with sparse, high-dimensional text features produced by TF-IDF and provides a useful benchmark for sentiment classification.

2. Multinomial Naive Bayes

Multinomial Naive Bayes is a probabilistic classification algorithm commonly used for text classification. It estimates class probabilities based on the distribution of words in the training data.

Both models are trained using the same training and test split to ensure a fair comparison.

📊 Model Evaluation Metrics

The trained models are evaluated using the following metrics:

Metric

Purpose

Accuracy

Measures the proportion of correctly classified reviews.

Precision

Measures how many reviews predicted as a particular sentiment actually belong to that class.

Recall

Measures how many reviews belonging to a sentiment class are correctly identified.

F1-score

Balances precision and recall using their harmonic mean.

Confusion Matrix

Shows correct and incorrect predictions for each sentiment class.

For a potentially imbalanced dataset, macro-averaged F1-score is particularly useful because it gives equal importance to each sentiment class.

🏆 Model Comparison and Best Model Selection

The performance of Logistic Regression and Multinomial Naive Bayes is compared using the evaluation metrics calculated on the held-out test dataset.

The best-performing model is selected based on its overall classification performance, with particular attention to macro F1-score, precision, recall, and the confusion matrix.

Logistic Regression may perform better when the relationship between TF-IDF features and sentiment classes is well captured by its decision boundaries. Multinomial Naive Bayes may offer faster training and strong baseline performance on word-frequency-based text features.

Note: The final best model will be determined from the actual experimental results. No model is assumed to perform better before evaluation.

🔍 Side-Effect Mining

The project also explores the identification of possible side-effect mentions in patient reviews using text analysis.

Potential approaches include:

Extracting frequent words and phrases from reviews.

Identifying adverse-effect-related terms using a predefined medical vocabulary.

Examining review text for mentions of symptoms or unwanted drug effects.

Summarizing frequently reported terms for further investigation.

This component is exploratory and does not establish that a drug caused a particular symptom. Patient reviews alone cannot confirm medical causality.

📈 Expected Outputs

The notebook is expected to generate:

Dataset overview and missing-value analysis.

Sentiment distribution visualizations.

Preprocessed review text and TF-IDF features.

Trained Logistic Regression and Multinomial Naive Bayes models.

Classification reports for both models.

A model performance comparison table.

Confusion matrices for both models.

A discussion of the best-performing model.

Exploratory side-effect-related terms and findings.

📌 Conclusion

This project demonstrates how Machine Learning and NLP can be applied to drug review analysis. By comparing Logistic Regression and Multinomial Naive Bayes, the project evaluates different approaches to sentiment classification and identifies the most suitable model based on measured performance.
