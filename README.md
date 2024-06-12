This project focuses on evaluating various methods for handling missing data in the context of HIV clinical research. The dataset used originates from the Lake Study, which involves monitoring various clinical and laboratory parameters of patients living with HIV. The primary goal is to compare different imputation techniques to determine the most effective method for managing missing values, ensuring robust and reliable statistical analyses.


In this study, four main methods for handling missing data were implemented and evaluated:

- Row Deletion (Eliminación de Filas): Removing rows with missing values.

- Simple Imputation (Imputación Simple): Imputing missing values using the median. 

- Modeling for Imputation (Modelado para Imputación): Predicting missing values using a preliminary model.

- Multiple Imputation (Imputación Múltiple): Using IterativeImputer for multiple imputation.

These methods were evaluated using a Random Forest model, and the performance was compared based on Root Mean Square Error (RMSE).

*Code Explanation* ->
The code is structured to perform the following tasks:

Data Preprocessing:

Loading the dataset.
Performing initial data cleaning and transformation.
Visualizing missing data patterns.
Missing Data Handling:

Implementing row deletion.
Applying simple imputation with the median.
Using a preliminary Random Forest model to predict and impute missing values.
Applying multiple imputation using IterativeImputer.
Model Training and Evaluation:

Separating features and target variable.
Training a Random Forest model for each imputation method.
Evaluating the model using cross-validation and calculating RMSE.
Visualization:

Creating bar plots to compare RMSE of different imputation methods.
Generating a heatmap to show correlations between CD4 counts and other variables.
