# Bank-Customer-Churn-Prediction-Model

## Project Overview
This project focuses on designing and training a neural network model to predict customer churn for a bank. The model identifies customers likely to leave within the next six months based on their attributes. The primary goal is to maximize accuracy and F1 score.

## Dataset
The dataset contains 10,000 samples with 14 features, including:
- `CustomerId`, `Surname`, `CreditScore`, `Geography`, `Gender`, `Age`, `Tenure`, `Balance`, `NumOfProducts`, `HasCrCard`, `IsActiveMember`, `EstimatedSalary`, and the target variable `Exited`.

## Key Steps
1. **Data Preprocessing**:
   - Handled missing data and categorical encoding.
   - Scaled features for consistent input to the model.
2. **Model Building**:
   - Constructed a neural network using Keras.
   - Included regularization techniques like Dropout to prevent overfitting.
   - Implemented early stopping for efficient training.
3. **Evaluation**:
   - Achieved an accuracy of 82% and an F1-score of 0.60 for the churn class.
   - Confusion Matrix:
     ```
     [[1375  232]
      [ 126  267]]
     ```

## Model Performance
- **Test Accuracy**: 82%
- **Test AUC**: 0.8478

## Insights
The model performs well in identifying non-churn customers but shows room for improvement in predicting churn. Class balancing and further hyperparameter tuning could enhance recall and F1-score.

## Future Enhancements
- Utilize advanced techniques such as ensemble methods.
- Optimize class weights or apply SMOTE for better handling of class imbalance.

---

### Repository Structure
- `Neural_Network_Model.ipynb`: Main notebook for data preprocessing, model training, and evaluation.
- `Neural_Network_Model.html`: HTML version of the project notebook.
- `README.md`: Overview of the project.

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/richardk100/Bank-Customer-Churn-Prediction-Model.git
   ```
2. Open the notebook in Google Colab or Jupyter Notebook.
3. Follow the steps to train and evaluate the model.

## License
This project is licensed under the MIT License.

Feel free to contribute or raise issues for further improvements!
