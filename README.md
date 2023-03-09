# Titanic-Challenge-Kaggle 🛳️⚓
This code is an implementation of the **Random Forest Classifier** 🌲 machine learning algorithm for the Titanic dataset, which predicts whether a passenger survived the sinking of the Titanic or not.

**Libraries Used**📚

**numpy** - a library for numerical computing in Python 🧮

**pandas** - a library for data manipulation and analysis 🐼

**sklearn** - a library for machine learning in Python 🤖

**Data Loading** 🔃

The **train_data** and **test_data** variables are created to load the training and testing data from the **train.csv** and **test.csv** files, respectively.

**Exploratory Data Analysis** 🔍

The percentage of women and men who survived the Titanic disaster is computed and printed to the console.

**Feature Engineering** ⚙️

The **features** variable contains a list of features used to train the Random Forest Classifier, namely **Pclass**, **Sex**, **SibSp**, and **Parch**. These features are transformed into numerical values using one-hot encoding through the **pd.get_dummies()** function.

**Model Training and Prediction** 🔮

The Random Forest Classifier is trained on the transformed features and survival data from the training dataset using the **RandomForestClassifier()** function. The **n_estimators** parameter specifies the number of trees in the forest, while **max_depth** specifies the maximum depth of each tree.

The model is then used to predict the survival of passengers in the test dataset using the **predict()** function.

**Submission** 📄

The predictions for the test dataset are saved in a **submission.csv** file using the **pd.DataFrame()** function, with columns **PassengerId** and **Survived**. Finally, the script prints a message to confirm that the submission was saved successfully.
