# Food Delivery Time Prediction

## Introduction

This project aims to predict the delivery time for food orders placed through a food delivery service, using data collected from ![Statso](https://statso.io/food-delivery-time-prediction-case-study/). The model uses various features such as restaurant location, order type, order time, distance from restaurant to customer location, delivery partner's age, previous ratings to predict the delivery time.

## Data

The data for this project was collected from ![Statso](https://statso.io/food-delivery-time-prediction-case-study/), and includes information such as previous delivery time, location, delivery partner's age, previous ratings and type of food. The data was preprocessed to handle missing values, outliers, and categorical variables.

## Model

The model was built using a combination of Sklearn, Keras and Tensorflow. The various features were fed into the model and linear regression, Random Forest, XGBoost, LightGBM were used to predict the delivery time. But to achieve a better result we used a Long Short-Term Memory (LSTM) Neural Network model, which is a type of Recurrent Neural Network (RNN) that is able to capture patterns in sequential data.

The model is created using the Sequential API of Keras. It has two LSTM layers and one dense layer. The input shape of the model is the shape of the training data. In the model, we have used Adam Optimizer and 'mean_squared_error' as the loss function. The model is trained using the `model.fit()` method with the batch size of 1 and epochs=9.

The model was evaluated using metrics such as MAE, MSE and R-squared.

## Results

The model achieved an accuracy of 97.333% on the test set, with a mean absolute error of Y minutes.

## Deployment

The model can be deployed as an API or integrated into an application to make the predictions available to users.

## Conclusion

This project demonstrates the potential of using machine learning to predict delivery times for food delivery services, which can help optimize routes and staffing, and provide more accurate delivery time estimates to customers.

## Requirements

- Python 3.8
- Sklearn, Keras, Tensorflow
- Numpy, Pandas
- Matplotlib (for data exploration and visualization)
