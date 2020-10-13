# machine-learning-challenge

Background
Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.
To help process this data, you will create machine learning models capable of classifying candidate exoplanets from the raw dataset.
In this homework assignment, you will need to:

Preprocess the raw data
Tune the models
Compare two or more models



Instructions

Preprocess the Data

Preprocess the dataset prior to fitting the model.
Perform feature selection and remove unnecessary features.
Use MinMaxScaler to scale the numerical data.
Separate the data into training and testing data.


Tune Model Parameters

Use GridSearch to tune model parameters.
Tune and compare at least two different classifiers.


Reporting

Create a README that reports a comparison of each model's performance as well as a summary about your findings and any assumptions you can make based on your model (is your model good enough to predict new exoplanets? Why or why not? What would make your model be better at predicting new exoplanets?).

Analysis

 A comparison of each model's performance.
 
I started off using linear models: SVM and LogisticRegression. I also looked through the data and selected features based on what sounded important. The scores and accuracy were less than 0.65 which lead me to add more features. The accuracy of the SVM and LogisticRegression models were both 0.81 which is below the desired accuracy of 0.85. This led to the selection of a RandomForestClassifier model which could handle more features and had a higher accuracy of 0.90.

A summary about your findings and any assumptions you can make based on your model (is your model good enough to predict new exoplanets? Why or why not?)

The RandomForestClassifier model was the best model selected to predict new exoplanets. I assumed that that less features would give higher accuracies, but it gave lower accuracies. After running the GridseachCV, there was no real optimizing the parameters the accuracy was steady. I ran a classification report and I am confident that the RandomForestModel is good enough to predict new exoplanets.

What would make your model be better at predicting new exoplanets?

The only thing I could think of to increase accuracy is adding a few more features. I could adjust a few more parameters but I wouldn’t expect an increase in accuracy.
