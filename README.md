# Deploying-Sentiment-Analysis-Project

This project is a sentiment analysis application that analyzes text data to determine whether the sentiment is positive, negative, or neutral. The model is deployed using AWS services, and a web interface is created using HTML for user interaction.

## Introduction

This project utilizes machine learning techniques to perform sentiment analysis on text data. The model is deployed on AWS, and users can interact with the model through a simple web interface.

## Features

- Sentiment analysis of text data
- Web interface for user interaction
- Model deployment using AWS services
- Real-time sentiment prediction

## Setup and Installation

### Prerequisites

- Python 3.6
- Jupyter Notebook
- AWS account
- HTML/CSS knowledge for web interface

## Deployment

### AWS Setup

#### Setting up Lambda Function:

- Create a new Lambda function in AWS Management Console. You can think it of as a straightforward Python function that can be executed whenever a specified event occurs. We will give this function permission to send and recieve data from a SageMaker endpoint. 
- Set up necessary IAM roles and permissions. Since we want the Lambda function to call a SageMaker endpoint, we need to make sure that it has permission to do so. To do this, we will construct a role that we can later give the Lambda function.

#### API Gateway:

- The method we will use to execute the Lambda function is a new endpoint that we will create using API Gateway. This endpoint will be a url that listens for data to be sent to it. Once it gets some data it will pass that data on to the Lambda function and then return whatever the Lambda function returns. Essentially it will act as an interface that lets our web app communicate with the Lambda function.
- Configure routes and methods to interact with the Lambda function.

#### Creating a Lambda Function:

- Using the AWS Console, navigate to the AWS Lambda page and click on Create a function and configure.

### Steps

1. Download or otherwise retrieve the data.
2. Process / Prepare the data.
3. Upload the processed data to Amazon S3.
4. Train a chosen model.
5. Test the trained model (typically using a batch transform job).
6. Deploy the trained model.
7. Use the deployed model.

## Technologies and AWS Services Used

- **Python**: For data processing and model training.
- **Jupyter Notebook**: For developing and experimenting with the model.
- **AWS Lambda**: For deploying and communicating with the model.
- **AWS API Gateway**: For creating APIs to communicate with the Lambda function and eventually with the trained model and back.
- **AWS S3**: For staging (storing) data.
- **HTML/CSS**: For the web interface.
