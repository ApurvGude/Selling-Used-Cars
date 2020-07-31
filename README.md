# Prediction model for Selling Used Cars

The Used cars market was valued at USD 25 billion in 2019 and it is expected to rise even more in the upcoming years.

As the number of used cars being sold is increasing it is important to know when it is the right time to sell your old car and buy a new one.

So, this project was made to predict when is the best time to sell your used cars, given the mileage range you will cover by that time.

The training data consists of selling prices of over 100000 used cars from 10 different car companies. Each used cars mileage,engine size, mpg, model and year sold was given too. The data was obtained from [here](https://www.kaggle.com/adityadesai13/used-car-dataset-ford-and-mercedes).

## [Part 1: EDA and Data Wrangling](https://github.com/ApurvGude/Selling-Used-Cars/blob/master/notebooks/PredictingUsedCarPrice.ipynb)

![Image 1](https://github.com/ApurvGude/Selling-Used-Cars/blob/master/images/index.png)

In this notebook, we analyzed each feature of the used car to see which factors affect the selling price of the cars. Based on these insights we wold make our first prediction model.

## [Part 2: Creating model to predict selling prices](https://github.com/ApurvGude/Selling-Used-Cars/blob/master/notebooks/Making%20the%20model.ipynb)

![Image 2](https://github.com/ApurvGude/Selling-Used-Cars/blob/master/images/index1.png)

In this notebook , we made a regression model to predict the selling price of a car.Many different models were tried and ensemble models turned out to give the highest accuracy. Of these models, we chose random forest regressor as our prediction model becasue of its high accuracy and low training time.

Random Forest Regressor on the validation set gave an R2 score of 0.96 with a RMSE of about 1000. This shows that the model was a very accurate regression model.

## [Part 3: Creating function to predict when and at which mileage to sell your used car](https://github.com/ApurvGude/Selling-Used-Cars/blob/master/notebooks/Making%20the%20model.ipynb)

In this part, based on the previous model we created a function which gave you the top 10 years and mileage values at which you could sell your car.

The user just has to input the features of the original car,the year range in which he wants to sell and the mileage range which he thinks he can maintain till selling time.
