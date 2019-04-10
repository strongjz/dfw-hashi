+++
title = "Development"
weight = 50
+++

{{< slide id="Development" background="#FFF" transition="zoom" transition-speed="fast" >}}


# Serverless Development

---

### Lambda setup 

There's three basic options for structuring this using AWS Lambda:

* Monolith  — One lambda function manages all the API actions.
* Service  — A single lambda function is responsible for a group of related actions. 
* Microservice — A single lambda function is responsible for only one action. 

---

### Lambda setup - Monolith

![](/dfw-hashi/images/arch.png)

---


### Lambda setup - Service


![](/dfw-hashi/images/services.png)

---

### Lambda setup - Microservice

![](/dfw-hashi/images/lambda-micro.png)

---


# Ngrok 

---

# Ngrok 

Spend more time programming. One command for an instant, secure URL to your localhost server through any NAT or firewall.

https://ngrok.com/product

---

# Ngrok 

![](/dfw-hashi/images/ngrok.png) 

---

# Ngrok 

![](/dfw-hashi/images/ngrok-running.png)

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


```bash
go get github.com/awslabs/aws-lambda-go-api-proxy/gin
```



---

# AWS Dynamodb Local

---


### AWS Dynamodb Local

![](/dfw-hashi/images/dynamodb.jpg) 


---

## AWS Dynamodb Local Running

```bash
docker run -p 8000:8000 amazon/dynamodb-local:1.11.477

```

---

# Deployment
