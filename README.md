# 💳 Credit-Card-Fraud-Detection-Model



### 🔍 Overview

This project focuses on detecting fraudulent credit card transactions using a machine learning approach. The dataset used contains transaction details including anonymized features, and the goal was to classify whether a transaction is fraudulent (1) or not (0).

Dataset used - https://www.kaggle.com/datasets/nelgiriyewithana/credit-card-fraud-detection-dataset-2023/data

### 🧠 What I Learned

Throughout this project, I learned how to:

- Understand and clean real-world datasets, including checking for missing values and irrelevant columns.
- Split data into training and testing sets for model evaluation.
- Apply **feature scaling** using `StandardScaler` to improve model performance.
- Train a **Random Forest Classifier**, a powerful ensemble method.
- Evaluate the model using classification metrics like **F1 score**, **precision**, **recall**, and **accuracy**.
- Use **cross-validation** to get a more reliable performance measure across multiple folds of data.
- Create helpful visualizations like:
- **Confusion Matrix** – to see how well the model classified fraud and non-fraud cases.
- **Feature Importance Plot** – to understand which features influence the model most.
- **Correlation Heatmap** – to explore relationships between features.
- **ROC Curve & AUC Score** – to measure the model’s ability to distinguish between the classes.

### 🤖 Model Used

I used a **Random Forest Classifier** with the following settings:

- `n_estimators=100`: Uses 100 trees in the forest.
- `max_depth=10`: Limits the depth of each tree to avoid overfitting.
- `min_samples_split=5`: A node must have at least 5 samples to be split.
- `n_jobs=-1`: Uses all CPU cores for training to speed up the process.

This model was trained using 5-fold cross-validation, and the **average F1 score** showed that the model performed well despite the dataset being imbalanced.

### 📊 Results

- The model showed strong performance in detecting fraudulent transactions, especially in terms of **precision**, which is crucial in fraud detection.
- The **ROC Curve** had a high AUC value, meaning the model does a good job distinguishing between fraud and non-fraud.
- The **feature importance plot** helped identify which variables were most important in decision making.

### 🧾 Final Thoughts

This project gave me a solid understanding of:

- Dealing with class imbalance in binary classification tasks.
- How Random Forest works and how to evaluate it properly.
- The importance of interpretability through visualizations.
- How small preprocessing steps like feature scaling can affect model performance.

This has been a great hands-on experience working with a real-world fraud dataset and applying practical machine learning skills to solve a problem that exists in the financial world.
