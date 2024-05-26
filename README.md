# Deploying-Sentiment-Analysis-Project
This project is a sentiment analysis application that analyzes text data to determine whether the sentiment is positive, negative, or neutral. The model is deployed using AWS services, and a web interface is created using HTML for user interaction.

# Introduction
This project utilizes machine learning techniques to perform sentiment analysis on text data. The model is deployed on AWS, and users can interact with the model through a simple web interface.

# Features
Sentiment analysis of text data
Web interface for user interaction
Model deployment using AWS services
Real-time sentiment prediction
Setup and Installation
Prerequisites
Python 3.x
Jupyter Notebook
AWS account
HTML/CSS knowledge for web interface

# Deployment
AWS Setup
Lambda Function:

Create a new Lambda function in AWS Management Console.
Upload the trained model and the handler code.
Set up necessary IAM roles and permissions.
API Gateway:

Create a new API in API Gateway.
Configure routes and methods to interact with the Lambda function.
S3 Bucket:

Create an S3 bucket to host your static website.
Upload the HTML, CSS, and JavaScript files to the bucket.
Steps
Train and save the sentiment analysis model.
Deploy the model to AWS Lambda.
Set up API Gateway to trigger the Lambda function.
Host the HTML page on S3.
Technologies Used
Python: For data processing and model training.
Jupyter Notebook: For developing and experimenting with the model.
AWS Lambda: For deploying the model.
AWS API Gateway: For creating RESTful APIs.
AWS S3: For hosting the web interface.
HTML/CSS: For the web interface.
