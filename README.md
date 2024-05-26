# Decision Tree Classifier

This code implements a decision tree classification algorithm. It can be used for tasks like predicting car prices based on features such as model, year, transmission type, fuel type, and manufacturer.

### Key Features:

- Handles both continuous and categorical features.
- Uses label encoding for categorical data.
- Handles missing values with simple imputation.
- Calculates information gain to choose the best split feature at each node.
- Outputs predictions on unseen data.

### How to Use:

1. Import libraries:
   <br> Import libraries like pandas (pd), scikit-learn (sklearn), and others as needed for data manipulation and preprocessing.
3. Load data: Load your training data as a pandas DataFrame (df). 
4. Preprocess data:<br> 
    - Encode categorical features using label encoding.
    - Handle missing values using imputation techniques.
    - Define feature names (feature_names) as a list of column names in your DataFrame.
5. Create a DecisionTree object:<br> 
    - Initialize a DecisionTree object with:
        - all_labels: Unique values for the target variable (e.g., car prices).
        - label_encoders: Dictionary containing label encoders for categorical features.
        - initial_allowed_features: List of all feature names.
        - target_idx: Index of the target variable in your DataFrame.
        - (Optional) Other parameters like min_sample_in_leaf for minimum samples per leaf node.
6. Train the tree:<br> 
    Call the create_tree method with your training data (data) as a NumPy array and allowed_features_idxes as a list of indices for allowed features (usually all features).
7. Test the tree: <br> 
    - Load your test data as a pandas DataFrame (test_data).
    - Encode categorical features in the test data using the same encoders used for training.
    - Call the test method with the test data as a NumPy array. This will return predicted labels for the test data. <br>
      
#### Additional Notes:
   The code can be further enhanced with features like hyperparameter tuning, visualization of the decision tree, and other evaluation metrics.
  Refer to the code for details on specific functions and their implementation.
