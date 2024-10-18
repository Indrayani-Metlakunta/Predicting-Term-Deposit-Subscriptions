

## Bank Term Deposit Prediction

### Problem Statement:
Build a Decision Tree classifier to predict if a client will subscribe to a term deposit based on their demographic and behavioral data.

### Dataset:
This dataset is from the UCI Machine Learning Repository and contains data related to direct marketing campaigns of a Portuguese banking institution. It aims to predict if a client will subscribe to a term deposit.

[Bank Marketing Dataset - UCI ML Repo](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)

### Key Features:
- **Demographics**: Age, Job, Marital status, Education, etc.
- **Behavioral Data**: Contact history, Campaign participation, Loan details, etc.
- **Economic Data**: Employment variation rate, Consumer price index, Euribor rates, etc.
- **Target**: Whether the client subscribed to the term deposit (yes/no).

### Process Overview:
1. **Data Preprocessing**:
   - Cleaned data with no missing values.
   - Duplicate entries considered valid, as multiple campaigns targeted the same clients.

2. **Exploratory Data Analysis**:
   - Age: Clients aged 30-40 most likely to subscribe.
   - Job: Admin, blue-collar, and technician roles showed higher subscription rates.
   - Education: Higher education correlated with higher subscriptions.
   - Loans: Clients with housing loans subscribed more, while personal loan holders subscribed less.

3. **Model Building**:
   - Implemented a Decision Tree classifier.
   - Achieved ~91.52% accuracy on both training and testing data.
   - Cross-validation score: ~91.60%.
   - Balanced precision, recall, and F1-scores.

4. **Key Insights**:
   - Call duration was a significant predictor—longer calls led to more subscriptions.
   - Previous contact attempts increased the likelihood of subscription.

### Future Work:
- Explore ensemble models to boost performance.
- Mitigate multicollinearity with feature selection methods.
- Consider external economic data for further improvements.

