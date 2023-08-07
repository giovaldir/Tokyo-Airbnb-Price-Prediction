## Tokyo Airbnb Price Prediction
- dataset : http://insideairbnb.com/


#### Programming Languages

  <img align="left" alt="Python" width="26px" src="https://raw.githubusercontent.com/rhoit/mode-icons/dump/icons/python.png" />
  <img align="left" alt="HTML5" width="26px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/html/html.png" />
  <img align="left" alt="CSS3" width="26px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/css/css.png" />
  <img align="left" alt="Terminal" width="26px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/terminal/terminal.png" />

<br />
<br />

![](tokyo-wallpaper.jpg)

## PROBLEM STATEMENT

"Tokyo Airbnb Price Prediction" is an analysis and prediction project focused on the Airbnb accommodation prices in Tokyo, Japan. Airbnb has become one of the most popular platforms for travelers and tourists to find unique and affordable places to stay during their visits to Tokyo. However, when it comes to comparing prices and determining the right value for a property on Airbnb, it can be a challenging task.

The main objective of this project is to develop an accurate price prediction model for Airbnb accommodations in Tokyo. The model will be based on historical data from the Airbnb website, including information about properties such as location, accommodation type, size, amenities, and previous guest reviews. By combining this data, we will leverage data analysis techniques and machine learning algorithms to build a model capable of predicting accommodation prices based on specific features.

## GOALS

- To conduct an analysis on the growth of Airbnb located near the venues to be used in the 2020 Olympics (using pandas, folium, seaborn, matplotlib, wordcloud).
- To predict Airbnb prices using Supervised Learning Regression as the key to renting out Airbnb and maximizing profits.
- To provide recommendations on Airbnb space using a Content-Based Recommendation System, helping existing Airbnb entrepreneurs to optimize their profits by obtaining the best specifications based on the top 5 most profitable areas.

## STEPS
The key steps in the "Tokyo Airbnb Price Prediction" project include:

- Data Collection: Gathering historical data related to Airbnb accommodations in Tokyo, including information about prices, locations, accommodation types, and other features.

- Data Cleaning: Performing data cleaning and preprocessing to handle missing or invalid values and identify and address outliers.

- Data Exploration: Conducting exploratory analysis to understand the relationships between variables and gain insights into the data characteristics.

- Modeling: Implementing various machine learning techniques such as linear regression, nonlinear regression, or deep learning algorithms to build the price prediction model.

- Model Evaluation: Evaluating the model's performance using relevant metrics such as Mean Absolute Error (MAE) or Root Mean Squared Error (RMSE).

- Conclusion and Interpretation: Interpreting the prediction results to gain insights into the factors influencing Airbnb accommodation prices in Tokyo.

## DATASETS

![](https://github.com/giovaldir/Predicting-Airbnb-Prices-using-Regression/blob/d5ba15952c9324d480b2b9a71e5b24993659ff8a/Screenshot%20(1488).png)
### METHODS
The method used in this project is regression, which aims to predict the price of Airbnb rentals in Tokyo based on factors such as location, amenities, room type, number of bedrooms, and more. I chose regression for this project because, as I learned from "Machine Learning Specialization by Andrew NG (Stanford)," it is perfect for predicting a numerical value from infinitely many possible values, which is precisely the task at hand in this project: predicting the price of an Airbnb rental.

#### REGRESSION
*Regression* is a statistical method used to estimate the association relationship between a dependent variable (Y) and one or more independent variables (X1, X2, X3, ..., Xn), relationship can be linear or non-linear and it usually has continuous output. 

- Dependent variable (response variable) -> measures an outcome of a study

- Independent variable (explanatory variables) explain changes in a response variable

Purpose of regression -> predict the value of dependent variable given the values of independent variables.

Why we need Regression ? helpful when companies would like to know about related factors that have significant impact on their key performance indicators. it also helps to create a new hypothesis that assist companies to improve their performance and hence better decision making

Types of Regression:
- Simple Regression -> One independent variable: Linear and non-linear

Y = B1X + B0 + E or some source mentioned Y = AX + B

    Y -> dependent variable
    B0 -> population Y-intercept/titik potong (naik turun garis linear)
    B1 -> population slope (kemiringan garis)
    X1 -> independent variable
    E -> Random error

- Multiple Regression -> More than one independent variable: linear and non-linear (X1, X2, X3, ..., Xn)

Y = B1X1 + B2X2 + B3X3 + ... + BkXk + B0 + E

Simple Linear vs Multiple Linear 

In SLR, we have one dependent variable (price) and one independent variable (size). If we want to determine the effect of the dependent variable (output) on more than one independent variable (input data, also known as predictors), we need to use Multiple Linear Regression (MLR). There is also Polynomial which is used to capture non-linear relationships between variables, where this regression uses quadratic functions. However, many mathematics professors also say that a polynomial function is linear if it has an order or degree of 1, and anything above that is considered non-linear.

When to use simple, multiple, and polynomial regression ? 

Actually it depends on the question we want to answer. If we want to find the relationship between one dependent variable and one independent variable, we can use simple or polynomial regression. If we want to find the relationship between one dependent variable and multiple independent variables, we use multiple linear regression.

So, if we only want to find the relationship with one independent variable, when should we use simple and when should we use polynomial regression? 

The answer is based on how well our model fits the original data. If a simple linear regression model already fits well, then it is sufficient to use that model alone. However, if it doesn't fit well and the function looks like a polynomial function (quadratic function), then we can try to approximate it using the polynomial regression method. There are several types of Regression Algorithms in ML, including:

- Linear Regression [more about](https://github.com/giovaldir/Predicting-Airbnb-Prices-using-Regression/blob/550f19688578df745a5106a277222c3c7437428f/Linear_Regression.ipynb)
- Polynomial Regression
- Random Forest Regressor
- Super Vector Regressor
- Decision Tree Regressor
- XGB Regressor
- and etc.


#### COST FUNCTION
The cost function, also known as the loss function or error function, is a function used to determine the difference between the predicted output generated by a mathematical model and the actual output. One example of this in regression cases includes:

- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- and etc.

The output of the Cost function is a decimal number that indicates the difference between the predicted output and the actual output (sometimes also called the target output) as described above. The larger the value of the Cost function, the greater the cost, loss, or error of the model used.
Ideally, the Cost Function value of a model is zero (0), which means that the predicted output is the same as the actual output. However, in reality, many factors make this ideal condition difficult to achieve, such as data distorted by noise, incomplete information, and so on. Therefore, what is done is to minimize the cost/loss/error, where if the result of the Cost Function approaches zero, the model will have better performance in predicting future outcomes.

If the predicted value and the output are far apart, optimization is needed, one of which is using Gradient Descent.

### EXPLORATORY DATA ANALYSIS (general)
The process of analyzing data to gain insights using methods such as visualizations and tables to maximize understanding and test hypotheses.

#### Neighbourhood

![](Neighbourhood-2.png)


#### Numerical Univariate Visualization

![](Numerical-2.png)


#### Categorical Univariate Visualization

![](Categorical-2.png)

#### Amenities
<a href="https://github.com/giovaldir"><img src="https://github.com/giovaldir/FINAL-PROJECT-TOKYO-AIRBNB/blob/master/Screen Shot 2020-09-15 at 13.50.40.png" width="500" height="500" alt="GiovaldiRC" ></a>

### To conduct an analysis on the growth of Airbnb located near the venues to be used in the 2020 Olympics (using pandas, folium, seaborn, matplotlib, wordcloud).
- I created a new column called "position", based on the proximity of the neighbourhood to the Stadium location. It was divided into three categories for easier understanding, namely close, medium, and far. The number of close locations was slightly higher than the others. Based on research, it can be concluded that Airbnb locations close to the Stadium have a very rapid increase in the number of bookings per year. For the last 3 years, 2017, 2018, and 2019, the numbers have continued to rise to 857, 1548, 1800 respectively. And for 2020, which only has data up to the 4th month, it has already reached 510, or 1/3 of 2019.
- For the average price, for those located close to the Stadium, it has been steadily increasing every year, but the most significant increase was seen in the last two years, 2019-2020, which was 30%. When converted to rupiah, it's around 477,680.
- In 2020, the accommodations themselves for locations that are close increased by 11% from 2019, and by 48% from 2018, a nearly two-fold increase.
- For bedrooms, from 2019, the price for a single room has increased by 7-8%. The most expensive area is currently Shibuya, with an average price of 26,317/3 million rupiah. Who doesn't know Shibuya? Shibuya Crossing is the busiest pedestrian crossing in the world, nicknamed the 24-hour non-stop area. The top 5 areas are Shibuya Ku', 'Shinjuku Ku', 'Toshima Ku', 'Taito Ku', 'Sumida Ku, all of which are equally interesting, with Shibuya being the most expensive.

### To predict Airbnb prices using Supervised Learning Regression as the key to renting out Airbnb and maximizing profits.
### EVALUATION METRICS
- R2, MAE,MSE,RMSE

| Algorithm | R square | MAE | MSE | RMSE | 
| --- | --- | --- | --- | --- | 
| XGBoost | 0.78 | 0.2 | 0.2 | 0.4 |
| Linear Regression | 0.72 | 0.3 | 0.3 | 0.5 |
| Polynomial Regression | 0.61 | 0.2 | 0.2 | 0.4 |
| SVR | 0.75 | 0.3 | 0.3 | 0.5 |
| Decision Tree | 0.67 | 0.4 | 0.4 | 0.6 |
| Random Forest | 0.74 | 0.2 | 0.2 | 0.4 |

- Based on my modeling, I found that the best algorithm model is XGBoost compared to others.
- Based on the above search results, the R square score is quite good, which is 0.78, indicating accuracy in predicting the actual value or accuracy in the case of classification.
- Based on the above results, the MSE is satisfactory to me because MSE indicates the error obtained from the difference between the actual and predicted values, squared. The smaller the error, the better the model.
- Based on the above results, the MAE is also very satisfactory to me because the MAE indicates the error obtained from the difference between the actual and predicted values, which is absolute, and it is good if it is small or close to 0.

### To provide recommendations on Airbnb space using a Content-Based Recommendation System, helping existing Airbnb entrepreneurs to optimize their profits by obtaining the best specifications based on the top 5 most profitable areas.
### RECOMMENDATION SYSTEM

The process of providing space recommendations by looking at Airbnb listings that have a review score rating of 100 in the most profitable areas/neighborhoods. The target of this recommendation is established Airbnb entrepreneurs who have been in business but have not been profitable enough. By providing this recommendation, the established Airbnb entrepreneur will know what the market likes, what specifications are actually needed for their Airbnb in that neighborhood, and of course, it will make it easier for the entrepreneur to improve their previous failures.

<a href="https://github.com/giovaldir/FINAL-PROJECT-TOKYO-AIRBNB/blob/master/8.FINAL%20PROJECT%20RECOMMENDATION%20SYSTEM%20CONTENT%20BASED-2.ipynb"><img src="https://github.com/giovaldir/FINAL-PROJECT-TOKYO-AIRBNB/blob/master/Recommendation System.png" alt="GiovaldiRC" ></a>
click for more information

### CONCLUSION

After examining the impact of the Minpaku Law, it is very apparent that there was a decrease in the number of Airbnbs, some neighborhoods were no longer able to participate in this business, and there was a decrease in prices in the years 2017-2018. However, with the 2020 Olympics, Airbnb as a sponsor was able to revive and become popular again. After 2018, prices continued to skyrocket, especially for those near the 2020 Olympics Venue. So, in terms of price impact, for entrepreneurs who want to start an Airbnb business, they should look at the proximity to the Venue as a promising factor, such as "Shibuya Ku', 'Shinjuku Ku', 'Toshima Ku', 'Taito Ku', 'Sumida Ku", which continue to experience increases of even up to 30% and continue to rise until the beginning of 2020. After obtaining various advantages of these locations according to Forbes, we can also see the trend of several types of rooms offered in Tokyo, two of which are promising, namely Entire home/Apt and Private room, which emphasize good privacy for visitors. Then, for experienced Airbnb entrepreneurs, from the results of the Recommender System, there are several Airbnbs that meet the criteria for spaces that can be used as references, which have the best ratings in some profitable areas. This can improve the business system of these experienced entrepreneurs. After all the needs for the place and specifications are fulfilled, don't forget about the details, such as some equipment that needs to be provided in your Airbnb in Tokyo, such as Heater, Washer, Wifi, Smoke Alarm, etc. With these things, price determination can be maximized and problems in this project can be solved.

### REFERENCES

- https://www.forbes.com/sites/sofialottopersio/2019/11/18/airbnb-olympic-partnership-ahead-ipo/#16377abb57a1
- https://www.businessinsider.com/airbnb-wins-reported-500-million-partnership-for-the-2020-tokyo-olympics-2019-11?r=US&IR=T
- https://www.nytimes.com/2019/10/01/travel/the-tokyo-2020-olympics-what-you-need-to-know.html
- https://mainichi.jp/english/articles/20180615/p2a/00m/0na/028000c
- https://phys.org/news/2018-06-airbnb-cancel-japan-law.html#:~:text=Rental%20site%20Airbnb%20said%20Thursday,for%20the%20%22extraordinary%20disruption.%22
- https://www.japantimes.co.jp/community/2018/04/01/how-tos/new-minpaku-law-will-alter-japans-rental-hospitality-landscape/
- https://www.olympic.org/tokyo-2020
- https://www.sakura-house.com/?gclid=CjwKCAjwzIH7BRAbEiwAoDxxTnL4DxKBxphjUND7Vgihq2WgdUgxd7Q4M723hEmUpErQp0KtV5-WtRoCrLcQAvD_BwE
- https://www.airbnb.jp/

### Thank You

[instagram]: https://www.instagram.com/giovaldirch
[linkedin]: https://www.linkedin.com/in/grm20222

[<img align="left" alt="giovaldir | LinkedIn" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/linkedin.svg" />][linkedin]
[<img align="left" alt="giovaldir | Instagram" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/instagram.svg" />][instagram]



<br />
<br />


