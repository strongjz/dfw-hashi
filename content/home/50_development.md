+++
title = "Development"
weight = 50
+++

# Serverless Development

---

### Lambda setup 

There's three basic options for structuring this using AWS Lambda:

* Microservice — A single lambda function is responsible for only one action. 
For example, there are 3 separate lambda functions for showing, creating and deleting a book.
* Service  — A single lambda function is responsible for a group of related actions. 
For example, one lambda function handles all book-related actions, but customer-related actions are kept in a separate lambda function.
* Monolith  — One lambda function manages all the bookstore actions.

---


# Ngrok 

---

### Stuff 

---

# AWS SAM
### Install [Guide](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html)

```
brew upgrade
brew update
brew tap aws/tap
brew install aws-sam-cli
```

---

### First, we install the Lambda go libraries

```bash
go get github.com/aws/aws-sdk-go
```
```bash
go get github.com/aws/aws-lambda-go/events
```
```bash
go get github.com/aws/aws-lambda-go/lambda
```

### Next, we install the core library
```bash
go get github.com/awslabs/aws-lambda-go-api-proxy
```

---

### Stuff 

---

# AWS Dynamodb Local

---

### Stuff 

---

# Deployment

---

### Stuff 
