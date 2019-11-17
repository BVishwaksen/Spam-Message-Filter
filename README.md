# Spam-Message-Filter
A machine learning based system that is used to predict whether the given message is spam(misleading message) or ham(true message).
## Table of Contents
[Introduction](#Introduction)
[Requirements](#Requirements)
[How-To-Use](#How-To-Use)
[Dataset](#Dataset)
[Technical-Details](#Technical-Details)
[Algorithm](#Algorithm)
[Lisence](#Lisence)
### Introduction
Messages are the most common form of communication. In our day to day life we send and receive a lot of messages. If all are real users and they send real  and necessary messages then there wont be no problem. But some of the attackers are using these messages to spread virus and to attack the systems and to penetrate into the user accounts. These messages are false by nature and technically called as spam messages. To establish more security to the user data we need to identify these spam messages and maintain a seperate record for them. As there are more number of users and messages for a specific communication platform it will be difficult to manually identifying the spam messages and it is not suggestable as it violates data confidentiality principles. In the pre machine learning era people used different technologies but the accuracy is less. So the idea of this project is to design a machine learning based system that can conclude whether the given message is spam or ham. 
### Requirements
Python 3.5 or above version with numpy,pandas,matplotlib,scikit-learn,seaborn and pickle packages.
Jupyter lab/Jupyter notebook
No specific hardware requirements and runs on any operating system
### How-To-Use
After downloading and extracting the repository open it in jupyter notebook.Then open the `spammessage_predictor.ipynb` file. In that file change the content of `message` variable with the message to be classified and then run all the cells.The type of the message is displayed as output of the last cell.

### Dataset
The dataset used in this project is SMSSpamCollection dataset from UCI Machine Learning repository
The dataset can be downloaded from <https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection>
### Technical-Details
##### Dataset Details
The dataset contains 2 attributes and 5574 instances.
The column details are
message type - (This variable is the target variable and has only two values spam or ham)
message - (This is the actual content of the meassge.The length of the message may vary.The maximul length of message is 8713 and this is fixed as the maximum size of the message)
##### Files Organization
The project is implemented in python in Jupyter Notebook environment.It mainly contains two parts.The `spammessage_trainer.ipynb` is for training the data and the `spammessage_predictor.ipynb` is to load the trained data and to predict results.The `heartdisease_model.sav` is the model that is saved.The `SMSSpamCollection` is the file that contains the dataset and we are using this dataset with tab seperation.
### Algorithm
The Heart Disease Prediction is a type of classification problem.As here there are only two types of target values `spam` or `ham` this comes under `binomial classification`.
The algorithm used in this is `Logistic Regression`.More details about this algorithm can be found at <https://en.wikipedia.org/wiki/Logistic_regression>
### Lisence
This is a public repository and you can be used in research,commercial and non-commercial applications without any restrictions.

