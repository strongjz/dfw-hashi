+++
title = "AWS"
weight = 40
+++

# AWS Serverless Application Model (SAM)

---

### AWS SAM

AWS SAM template specification 

```yaml
   Transform: 'AWS::Serverless-2016-10-31'
   Resources:
   
     ThumbnailFunction:
       # This resource creates a Lambda function.
       Type: 'AWS::Serverless::Function'
       
       Properties:
         
         # This function uses the Nodejs v6.10 runtime.
         Runtime: nodejs6.10
           
         # This is the Lambda function's handler.
         Handler: index.handler
         
         # The location of the Lambda function code.
         CodeUri: ./src
         
         # Event sources to attach to this function. In this case, we are attaching
         # one API Gateway endpoint to the Lambda function. The function is
         # called when a HTTP request is made to the API Gateway endpoint.
         Events:
   
           ThumbnailApi:
               # Define an API Gateway endpoint that responds to HTTP GET at /thumbnail
               Type: Api
               Properties:
                   Path: /thumbnail
                   Method: GET
```

---

### AWS SAM CLI

[Reference](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-command-reference.html)

* sam build
* sam deploy
* sam init
* sam local generate-event
* sam local invoke
* sam local start-api
* sam local start-lambda
* sam logs
* sam package
* sam publish
* sam validate

---

### AWS SAM CLI

* sam local generate-event
* sam local invoke
* sam local start-api
* sam local start-lambda

---


# Lambda

---

### Lambda

"AWS Lambda is a compute resource that runs your code in response to events and automatically manages the compute resources
for you, making it easy to build applications that respond quickly to new information"

---


### Lambda

* Code: s3
* Metadata: DynamoDB
* Execution: EC2 instances
* Permissions: IAM Roles

---

### Lambda

* Function
* Resources Allocation
* Code 
* Event
* Trigger

---

### Lambda

"Run and forget"

---

### Lambda

Drawback: Does NOT respond to HTTP Events

---

# AWS API Gateway

---

### AWS API Gateway 

* Create REST APIs
* Create WebSocket APIs

---

### AWS API Gateway 


* Endpoint
* Methods
* Integration - Backend
 
---

### AWS API Gateway Integrations

* Lambda
* HTTP 
* S3 Proxy
* Kinesis Proxy

---

### AWS API Gateway Endpoints

* Edge Optimized 
* Regional 
* Private API

---

### AWS API Gateway Methods

* HTTP Method
* Request Parameters
* Request Model
* Request Authorization
* Request Validation


---

### AWS API Gateway Authorization

 * including IAM roles and policies (AWS_IAM)
 * an Amazon Cognito user pool (COGNITO_USER_POOLS), 
 * or a Lambda authorizer (CUSTOM)

--- 

# Dynamodb

---

### Dynamodb 

Serverless Web scale NOSQL AWS managed database. 

---

# S3

---

### s3 

Web Scale Storage


