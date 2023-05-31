# Advanced Topics in GIScience Spring 2022
## Assignment #2

### @1

**About:** The Californian Housing Dataset is from the book *Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow* by Aurelien Geron. It contains district-based housing data combined with the median house prices of the district.

**The columns of the dataset are:**
  1. longitude: The longitude coordinate of the district.
  2. latitude: The latitude coordinate of the district.
  3. housing_median_age: The median age of houses in the district.
  4. total_rooms: The total number of rooms in the district's houses.
  5. total_bedrooms: The total number of bedrooms in the district's houses.
  6. population: The total population of the district.
  7. households: The total number of households in the district.
  8. median_income: The median income of households in the district.
  9. median_house_value: The median value of houses in the district.

**[Fastai TabularModel](https://docs.fast.ai/tabular.model.html)**

The design of the model deployed within this notebook was led by Jeremy Howard and Sylvain Gugger, the creators of Fastai. The architecture consists of multiple layers of fully connected neural networks, also known as dense layers. These layers process the input features of the tabular data and learn to extract relevant patterns and relationships from the data.

**[Random Forest](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)**

Random Forest is an ensemble learning method that combines multiple decision trees to make predictions. It is based on decision trees. A decision tree is a flowchart-like structure where each internal node represents a feature or attribute, each branch represents a decision rule, and each leaf node represents an outcome or prediction. Decision trees are created by recursively splitting the data based on the selected features until a stopping condition is met. Random Forest combines multiple decision trees that independently operate on a random subset of the input data and vote for a prediction result. The outcome prediction of a random forest regression is the average of every prediction from the decision trees.

**Problem:**

The goal of this notebook is to use Fastai to train a neural network and predict the housing prices of the district. Then compare a Random Forest Classifier with the network.

**Research Questions:**
1. What variables of the dataset have the largest impact on housing prices?
2. With what level of accuracy is it possible to predict the housing prices using the tabular neural network provided by Fastai?
3. What level of accuracy can be achieved with a naive implementation of a random forest regressor?
4. How does random forest compare to the neural network?

**Hypothesis:**

The location of the district as well as the ocean proximity will play a significant role in predicting the housing prices. This is assumed because places like San Francisco are commonly known for their high rent rate and house prices. The further away a district is from the logistical centers, the smaller the housing price.

The second hypothesis is that the neural network will outperform the random forest regressor. However, the difference will not be much. Given a sufficient amount of data and high-quality data, random forest has the potential to yield high accuracy results.
