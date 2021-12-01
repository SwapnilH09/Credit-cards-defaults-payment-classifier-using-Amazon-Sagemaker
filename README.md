# Project description
Working on a classification problem with the Defaults of credit card clients dataset https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients
provided by UCI using Amazon Sagemaker IDE.

## first commit 
1. upload dataset into a s3 bucket by defining its identifier and other parameters
2. created a script for processing job to process the data and generate features using Amazon Sagemaker Processing
3. runs the processing job and stores their outputs(prepared features) at mentioned location in s3 bucket

## second commit
1. create a sagemaker experiment(tracked under trials) to run a xgb classifier over the prepared data
2. set up a batch transform endpoint locally
3. define a function to pull the output of batch transform job
4. evaluate the model using accuracy_score and confusion matrix
5. compare the baseline model accuracy and the model accuracy(pre-trained xgb model provided by sagemaker team)
