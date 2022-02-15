# DetectingDepressionSocialMediaText-LT-EDI-ACL-2022
Repository of Code for the Shared task on Detecting Signs of Depression from Social Media Text at LT-EDI 2022- ACL 2022

This is the code submitted by team SSN for WORKSHOP ON LANGUAGE TECHNOLOGY FOR EQUALITY, DIVERSITY, INCLUSION at ACL-2022

This repository contains datasets obtained from the organizers of the shared task.
The link to the CodaLab competetion has been provided.

The brief description of the different models implemented is given below

Preprocessing (Common to all runs): 
Duplicates were dropped and labels were encoded in one hot notation.
Stop words were removed before tokenization with a vocabulary size of 1024 words.

Run 1: 
A simple Embedding layer passed on to 2 dense layers. 
Least complex model with  68,803 parameters. Trained for 30 epochs.

Run 2: 
A RNN with 2 Bidirectional LSTM layer passed on to 2 Dense layers. 
Dropout was used to avoid overfitting. This model has around 177,000 parameters. Trained for 5 epcohs.

Run 3: 
A transfer Learning model using BERT from TFHub. 
The output of BERT is passed to a Dense layer acting as a classifier. 
Most complex model of the 3 having over 28 million trainable parameters. Trained for 3 epochs.
