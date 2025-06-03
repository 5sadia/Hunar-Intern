# House Price Prediction using Linear Regression

This project implements a linear regression model to predict house prices based on various features of the houses. The analysis is performed in a Google Colab notebook.

## Project Structure

-   `house price data.csv`: The dataset used for training and evaluating the model.
-   `task2.ipynb`: The Colab notebook containing the code for data loading, cleaning, exploration, model training, and evaluation. (Replace `task2.ipynb` with the actual name of your notebook file)

## Dataset

The dataset contains information about houses and their corresponding sale prices. Key features used in the analysis include:

-   `sqft_living`: Square footage of the living area.
-   `sqft_above`: Square footage of the house above ground level.
-   `bathrooms`: Number of bathrooms.
-   `bedrooms`: Number of bedrooms.
-   `price`: The target variable, representing the house price.

Irrelevant columns such as `date`, `street`, `city`, `statezip`, and `country` were dropped during data preprocessing.

## Methodology

1.  **Data Loading and Cleaning:** The dataset is loaded into a pandas DataFrame. Irrelevant columns are removed, and missing values are handled by dropping the corresponding rows.
2.  **Exploratory Data Analysis (EDA):**
    -   A correlation heatmap is generated to visualize the relationships between different features and the target variable (`price`).
    -   Scatter plots are created to show the relationship between the top features (`sqft_living`, `sqft_above`, `bathrooms`, `bedrooms`) and the `price`.
3.  **Model Training:**
    -   The data is split into training and testing sets.
    -   A Linear Regression model from scikit-learn is initialized and trained on the training data.
4.  **Model Evaluation:**
    -   The trained model is used to make predictions on the test set.
    -   The performance of the model is evaluated using the following metrics:
        -   R² Score: Measures the proportion of the variance in the dependent variable that is predictable from the independent variables.
        -   RMSE (Root Mean Squared Error): Measures the average magnitude of the errors.
    -   The intercept and coefficients of the linear regression model are printed to understand the relationship between each feature and the price.
5.  **Visualization of Results:**
    -   A scatter plot of actual vs. predicted prices is generated to visually assess the model's performance. A red line representing perfect prediction is also plotted.
    -   A residual plot is created to examine the distribution of the errors (residuals).
    -   A histogram of the residuals is plotted to check for normality.

## Dependencies

The project requires the following libraries:

-   pandas
-   numpy
-   matplotlib
-   seaborn
-   scikit-learn

These dependencies are installed and imported within the Colab notebook.

## How to Run the Code

1.  Upload the `house price data.csv` file to your Google Drive or directly to your Colab environment.
2.  Open the `task2.ipynb` file in Google Colab.
3.  Run the cells in the notebook sequentially.

The notebook will perform the data loading, cleaning, model training, and evaluation steps, and display the results including visualizations.

## Results

The evaluation metrics (R² Score and RMSE) and the model coefficients are printed in the notebook. The visualizations provide further insight into the model's performance and the relationships within the data.

