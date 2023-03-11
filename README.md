#TITLE OF THE PROJECT: WEATHER FORECASTING PREDICTION
#BACKGROUND:For the current situation, India observatory conducts traditional weather forecasting. There are four common methods to predict the weather. The first method is the climatology method that is reviewing weather statistics gathered over multiple years and calculating the averages. The second method is an analog method that is to find a day in the past with weather similar to the current forecast. The third method is the persistence and trends method that has no skill to predict the weather because it relies on past trends. The fourth method is numerical weather prediction the is making weather predictions based on multiple conditions in the atmosphere such as temperatures, wind speed, high-and low pressure systems, rainfall, snowfall, and other conditions. So, there are many limitations of these traditional methods. Not only it forecasts the temperature in the current month at most, but also it predicts without using machine learning algorithms. Therefore, my project is to increase the accuracy and predict the weather in the future for at least one month by applying machine learning techniques.
#MOTIVATION:
1.	Improved Accuracy
2.	 Early Warning
3.	Business Applications
4.	Climate Change Mitigation
Overall, the motivation for using machine learning for weather forecasting is to improve the accuracy, reliability, and usefulness of weather forecasts for a range of applications, from public safety to business operations, to environmental protection.
#PROBLEM STATEMENT:The problem statement for weather forecasting using machine learning is to accurately predict weather conditions based on current and historical meteorological data. The goal is to improve the accuracy and reliability of weather forecasts, which can have significant implications for public safety, business operations, and environmental protection.
                  Overall, the problem statement for weather forecasting using machine learning is to develop accurate, reliable, and adaptable algorithms that can provide early warning of extreme weather events, help businesses make informed decisions, and contribute to efforts to mitigate the effects of climate change.
#DATA SET DESCRIPTION: In this project, we are concentrating on the temperature prediction of Kanpur city with the help of various machine learning algorithms and various regressions. By applying various regressions on the historical weather dataset of Kanpur city we are predicting the temperature like first we are applying Multiple Linear regression, then Decision Tree regression, and after that, we are applying Random Forest Regression.
#Existing solution:
•	IBM's Deep Thunder: Deep Thunder is a high-resolution weather forecasting system developed by IBM that uses machine learning algorithms to provide real-time weather forecasts. The system combines traditional numerical weather prediction models with machine learning techniques to improve forecast accuracy.
•	Google's Global Flood Forecasting Model: Google has developed a machine learning-based global flood forecasting model that predicts the likelihood and severity of flooding in real-time. The model uses satellite imagery and meteorological data to provide accurate predictions. 
•	The Weather Company: The Weather Company, a subsidiary of IBM, uses machine learning algorithms to provide weather forecasts for businesses and organizations. The company uses a range of data sources, including weather radar and satellite imagery, to provide highly accurate and detailed forecasts.
•	AccuWeather: AccuWeather is a weather forecasting company that uses machine learning algorithms to provide highly accurate weather forecasts. The company uses a range of data sources, including weather radar, satellite imagery, and weather station data, to provide real-time and accurate forecasts.
#Methodology:The dataset utilized in this arrangement has been gathered from Kaggle which is “Historical Weather Data for Indian Cities” from which we have chosen the data for “Kanpur City”. The dataset was created by keeping in mind the necessity of such historical weather data in the community. The datasets for the top 8 Indian cities as per the population. The dataset was used with the help of the worldweatheronline.com API and the wwo_hist package. The datasets contain hourly weather data from 01-01-2009 to 01-01-2020. The data of each city is for more than 10 years. This data can be used to visualize the change in data due to global warming or can be used to predict the weather for upcoming days, weeks, months, seasons, etc. Note: The data was extracted with the help of worldweatheronline.com API and we cannot guarantee the accuracy of the data. The main target of this dataset can be used to predict the weather for the next day or week with huge amounts of data provided in the dataset. Furthermore, this data can also be used to make visualization which would help to understand the impact of global warming over the various aspects of the weather like precipitation, humidity, temperature, etc. 
#Proposed Methodology:
 Table 1.1: Historical Weather Dataset of Kanpur City
![Screenshot 2023-03-11 204022](https://user-images.githubusercontent.com/127608346/224494984-79c1da1d-2044-4123-a3ff-e309baad8228.png)
Figure 1.1: Plot for each factor for 10 years
![blob](https://user-images.githubusercontent.com/127608346/224495024-387e36d6-bbb1-4086-9681-a3961d092a50.jpeg)
Figure 1.2: Plot for each factor for 1 year
![blob (1)](https://user-images.githubusercontent.com/127608346/224495043-a4a4515b-4e05-4d2f-aeb1-6a2d2ae795e2.jpeg)
#Implementation details:
          Multiple Linear Regression: This regression model has high mean absolute error, hence turned out to be the least accurate model. Given below is a snapshot of the actual result from the project implementation of multiple linear regression.
![Screenshot 2023-03-11 210058](https://user-images.githubusercontent.com/127608346/224495078-26517273-131f-45fa-90e4-c934b6e7fd15.png)
          Decision Tree Regression: This regression model has medium mean absolute error, hence turned out to be the little accurate model. Given below is a snapshot of the actual result from the project implementation of multiple linear regression.
![Screenshot 2023-03-11 210433](https://user-images.githubusercontent.com/127608346/224495123-707c4ac1-1e71-4fbe-850f-3da0a93f80d0.png)
          Random Forest Regression: This regression model has low mean absolute error, hence turned out to be the more accurate model. Given below is a snapshot of the actual result from the project implementation of multiple linear regression.
![Screenshot 2023-03-11 210709](https://user-images.githubusercontent.com/127608346/224495153-698dab01-c2df-4a1c-92ac-17f45e541642.png)
#Experimental results and evaluation:The record has just been separated into a train set and a test set. Each information has just been labeled. First, we take the trainset organizer. We will train our model with the help of histograms and plots. The feature so extracted is stored in a histogram. This process is done for every data in the train set. Now we will build the model of our classifiers. The classifiers which we will take into account are Linear Regression, Decision Tree Regression, and Random Forest Regression. With the help of our histogram, we will train our model. The most important thing in this process is to tune these parameters accordingly, such that we get the most accurate results. Once the training is complete, we will take the test set. Now for each data variable of the test set, we will extract the features using feature extraction techniques and then compare its values with the values present in the histogram formed by the train set. The output is then predicted for each test day. Now in order to calculate accuracy, we will compare the predicted value with the labeled value. The different metrics that we will use confusion matrix, R2 score, etc.
#Conclusion:All the machine learning models: linear regression, various linear regression, decision tree regression, random forest regression were beaten by expert climate determining apparatuses, even though the error in their execution reduced significantly for later days, demonstrating that over longer timeframes, our models may beat genius professional ones. Linear regression demonstrated to be a low predisposition, high fluctuation model though polynomial regression demonstrated to be a high predisposition, low difference model. Linear regression is naturally a high difference model as it is unsteady to outliers, so one approach to improve the linear regression model is by gathering more information. Practical regression, however, was high predisposition, demonstrating that the decision of the model was poor and that its predictions can't be improved by the further accumulation of information. This predisposition could be expected to the structure decision to estimate temperature dependent on the climate of the previous two days, which might be too short to even think about capturing slants in a climate that practical regression requires. On the off chance that the figure was rather founded on the climate of the past four or five days, the predisposition of the practical regression model could probably be decreased. In any case, this would require significantly more calculation time alongside retraining of the weight vector w, so this will be conceded to future work. Talking about Random Forest Regression, it proves to be the most accurate regression model. Likely so, it is the most popular regression model used, since it is highly accurate and versatile. Below is a snapshot of the implementation of Random Forest in the project. Weather Forecasting has a major test of foreseeing the precise outcomes which are utilized in numerous ongoing frameworks like power offices, air terminals, the travel industry focuses, and so forth. The trouble of this determining is the mind-boggling nature of parameters. Every parameter has an alternate arrangement of scopes of qualities.




