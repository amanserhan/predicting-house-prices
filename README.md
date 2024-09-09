# predicting-house-prices
This project involves predicting house prices in the United States using linear regression models. The dataset consists of over 2.2 million entries, including features such as the number of bedrooms, bathrooms, lot size, and house size. The main objective is to build and evaluate a linear regression model to accurately estimate house prices based on these features.

## Data

Link to dataset: https://www.kaggle.com/datasets/ahmedshahriarsakib/usa-real-estate-dataset/data

### Features

The dataset includes the following columns:

- **Brokered By**: The agent or agency handling the sale.
- **Status**: The current status of the property (e.g., for sale, sold).
- **Price**: The target variable representing the house's sale price.
- **Bed**: Number of bedrooms in the house.
- **Bath**: Number of bathrooms.
- **Acre Lot**: The size of the lot in acres.
- **Street**: The street name and number.
- **City**: The city where the house is located.
- **State**: The state where the house is located.
- **Zip Code**: The ZIP code of the area.
- **House Size**: The size of the house in square feet.
- **Previous Sold Date**: The last time the property was sold.

### Target

- **Price**: This is the target variable representing the house's sale price.

## Methods

### Data Preprocessing

- **Data Type Conversion**: The data types of various columns were corrected to ensure accurate analysis.
- **Missing Values**: The dataset was cleaned by addressing any missing values.
- **Feature Scaling**: Standard scaling was applied to the features to ensure that they were within a similar range.

### Model Selection

- **Linear Regression**: A simple linear regression model was implemented to predict house prices based on the `house_size` feature. The model was iterated to improve accuracy by adding more features such as the number of bedrooms and bathrooms.
- **Multiple Linear Regression**: An extended model was created using multiple features including `house_size`, `bed`, and `bath` to improve prediction accuracy.

### Model Evaluation

- **Train-Test Split**: The data was split into training and testing sets, with 80% used for training and 20% for testing.
- **Correlation Analysis**: The correlation between features such as `house_size` and `price` was analyzed to guide feature selection.
- **Evaluation Metrics**: The models were evaluated using the coefficient of determination (R^2) and Mean Squared Error (MSE) to assess their accuracy.

## Results

- **Best Model**: The linear regression model using `house_size` as a feature showed a strong positive correlation with `price`. However, adding more features like `bed` and `bath` provided only marginal improvements, suggesting that these features were not as strongly correlated with `price`.
- **Key Insights**: The model's accuracy highlights the importance of `house_size` as a significant predictor of house prices. Other features like the number of bedrooms and bathrooms had less impact on the accuracy of the model.

## Conclusion

This project demonstrates the application of linear regression to predict house prices. The results suggest that while house size is a key factor in determining price, the number of bedrooms and bathrooms are less significant. Future work could involve exploring additional features or experimenting with other types of models beyond linear regression to improve accuracy further.
