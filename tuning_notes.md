# Model Tuning Notes

The traditional machine learning models use `GridSearchCV` with F1-score as the selection metric.

The deep learning models use a small manual grid because FNN, LSTM, and CNN training is slower on a regular laptop than scikit-learn models. The script tests practical configurations for sequence length, embedding size, hidden units or filters, dropout, learning rate, and epochs. The intended selection metric is validation F1-score, then the selected configuration is saved as the final app model.

This keeps the project reproducible while still showing real tuning instead of leaving the deep learning models at random default settings.
