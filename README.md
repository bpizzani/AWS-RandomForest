# AWS-RandomForest


## About The Project
Preprocess data to train a deployed model to predicts Fraud using a XGBoost algorithm in AWS.


## Built With
•	AWS SageMaker
•	Python

## Getting Started
You will need access to Amazon Web Services Notebook instance and clone this project there. Open the terminal in the SakeMaker Notebook and type
```bash
cd SageMaker
git clone https://github.com/bpizzani/AWS-RandomForest.git
```

## Prerequisites
To build the model and preprocess the data you will need the following knowledge:

•	AmazonWebServices – SageMaker

•	API and Lambda functions

•	Machine Learning concepts

•	Sklearn

## Installation
1.	Clone the repo
```bash 
git clone https://github.com/bizzani/AWS-RandomForest.git
```
2.	Install pip packages:

•	Numpy

•	Pandas

```bash
pip install <packages>
```
  
## Usage
Once you have clone the project into ASW Sagemaker Notebook you can access the .ipynb file and run the preprocessing code and build the XGB model estimator and carry on the deployment. 

Once the predictor (estimator.deploy()) has been created we create a Lambda Function and invoke the endpoint setting the endpoint name to the predictor endpoint name (predictor.endpoint).

Lambda function code is also included in this project.

Finally, we create an API linked to our lambda function in AWS API, and we will get the API url that we would need to copy and paste into the “Index.html” file in the where: action= “link”

The lambda functions will take a string and convert it to a list of a single string since the model would accept an array in order to make predictions.
To make predictions we access “Index.html” and just type down our comment.

## License
Distributed under the MIT License. See LICENSE for more information.

## Contact
Your Name – bpizzani92@gmail.com
Project Link: https://github.com/bpizzani/AWS-RandomForest.git
