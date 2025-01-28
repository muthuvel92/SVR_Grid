# SVR_Grid
Notes from my learning on Step by step instruction for creating a Machine learning Model Medical Insurance Prediction using SVR Grid

### Summary of SVR Grid in Machine Learning

**Support Vector Regression (SVR)** is a powerful regression technique in machine learning that utilizes the principles of Support Vector Machines (SVM) to predict continuous values. When optimizing SVR models, a **Grid Search** is often employed to find the best hyperparameters that improve model performance.

#### Key Components of SVR Grid

- **Hyperparameters**: SVR has several hyperparameters that can significantly impact its performance, including:
  - **C**: Regularization parameter that controls the trade-off between achieving a low training error and a low testing error.
  - **Kernel**: The function used to transform the data into a higher-dimensional space (e.g., linear, polynomial, RBF).
  - **Gamma**: Defines the influence of a single training example. A low gamma means 'far' and a high gamma means 'close.' It affects the curvature of the decision boundary.

- **Grid Search**: This method systematically works through multiple combinations of hyperparameter values specified in a grid and evaluates the model's performance for each combination.
  - **Cross-Validation**: Often combined with grid search, cross-validation assesses the model’s performance on different subsets of the dataset, ensuring that the chosen hyperparameters generalize well to unseen data.
  
#### Steps in SVR Grid Search

1. **Define the Parameter Grid**: Create a dictionary containing the hyperparameters to optimize and their corresponding values.
2. **Instantiate the SVR Model**: Use the SVR class from libraries like Scikit-learn.
3. **Configure Grid Search**: Utilize tools like `GridSearchCV` from Scikit-learn to perform the search with specified scoring metrics (e.g., mean squared error).
4. **Fit the Model**: Train the model on the training data using the grid search.
5. **Evaluate Results**: Analyze the output to find the best-performing hyperparameter combination based on the defined scoring metric.
