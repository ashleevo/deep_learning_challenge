# deep_learning_challenge

Module submission for the University of California Berkeley Data Analysis Program
Assistance with completing the module can be attributed to course material from the program, StackOverFlow and ChatGPT for key error evaluation, and my own notes.

# Purpose

We performed a deep learning module that was aimed to predict whether or not applicants would be successful if funded by a non profit foundation, Alphabet Soup.

# Background
We were provided a CSV that contains more than 34,000 organizations recieving funding from Alphabet Soup. The columns are as follows:

EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special considerations for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively

# Data Preprocessing

Columns that were useful were pulled from the read in CSV. The columns EIN and NAME were dropped.

The APPLICATION_TYPE and CLASSIFICATION column were examined for binning purposes and cutoffs were established.

Additionally, categorical data was converted to numeric values in order for our model to perform, since categorical/object data cannot be used to perform calculations.

# Splitting and Training the Data

The target variable was identified as the IS_SUCCESSFUL column because we want to made predictions based upon the data in this column. The other columns are considered our features to examine that effects the success or failure outcome of the organization.

# Building the Model

Evaluations of implementing different layers and numbers of neurons were needed in order to optimize the model effectiveness. In the end, 80 and 30 neurons were implemented into the first and second hidden layers with a model loss of 0.567 and an accuracy of .7301

# Conclusion

With a 73% accuracy, the model performs acceptably but not completely precise. The model could be manipulated to be more precise by filtering down other columns that may not contribute as much to the success rate as predicted.

