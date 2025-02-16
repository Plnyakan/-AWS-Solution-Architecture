# Serverless Contact Form with API Gateway and Lambda

![diagram-export-2-16-2025-8_21_26-PM](https://github.com/user-attachments/assets/69174f6a-2b7f-424c-9efb-fffd5ed49350)


## Overview
This document provides instructions for setting up an API Gateway to receive form submissions, processing the data using AWS Lambda, storing it in DynamoDB, and sending email notifications using Amazon SES.

## Components
1. **API Gateway**: Accepts HTTP POST requests containing form submissions.
2. **AWS Lambda**: Processes the form data using Node.js.
3. **DynamoDB**: Stores the plain text data from form submissions.
4. **Amazon SES**: Sends email notifications to form submitters and system administrators.
## Prerequisites
- AWS account with necessary permissions.
- Basic knowledge of AWS services (API Gateway, Lambda, DynamoDB, SES).
## Setup Instructions
### API Gateway
1. **Create an API Gateway**:
    - Set up the API Gateway to handle HTTP POST requests.
    - Configure the endpoint to trigger the AWS Lambda function.
2. **Security Measures**:
    - Ensure IAM role permissions are correctly set up.
    - Enable SSL/TLS encryption for secure data transmission.
### AWS Lambda
1. **Function Creation**:
    - Create a Lambda function using Node.js.
    - Write the logic to process incoming form data.
2. **Integration with DynamoDB**:
    - Set up the Lambda function to store processed data in a DynamoDB table.
3. **Logging and Monitoring**:
    - Use CloudWatch to monitor logs and track the performance of the Lambda function.
### DynamoDB
1. **Table Setup**:
    - Create a DynamoDB table to store plain text data.
    - Define the necessary attributes and primary key.
### Amazon SES
1. **Email Configuration**:
    - Configure SES to send email notifications.
    - Set up recipient addresses for form submitters and system administrators.
## Monitoring and Maintenance
- Monitor system performance and logs using CloudWatch.
- Regularly review and update security settings as needed.
## 


