Imported Libraries: The notebook uses a variety of Python libraries for data processing, machine learning, and visualization:

Data Handling:
pandas
numpy


Machine Learning:
sklearn (e.g., LinearRegression, DecisionTreeRegressor, train_test_split, LabelEncoder, etc.)


Visualization:
matplotlib.pyplot
seaborn


Metrics:
r2_score
mean_squared_error


First we load data from a CSV file into a dataframe(using pd) and then display the first 5 rows to understand the dataset.
I checked for missing values and then dropped them if they exist(in this case, none). Then I created pair wise plots for all numeric datas for visualisation. We separate the independent and dependent variables by splitting them. Since there are categorical data in our dataset, I converted them into numeric format by making use of OneHotEncoder and dropping all the categorical data. After this, I split them into train and test by allotting 80% of our data for training and 20% of it for testing. For normalising the features for better performance, I used standard scaler. I used linear regression model to train and make the predictions. To evaluate the model, i used mean squared error metric. I also made an use of Decision tree model as an alternative to compare the results of the both and returned the result.