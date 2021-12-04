# AWS CLI Scripts

A collection of scripts and commands to use with AWS CLI

### Basic

- aws configure

### Lambda 

- aws lambda list-functions
- aws lambda create-function --function-name hello-node --zip-file fileb://function.zip --runtime nodejs14.x --role arn:aws:iam::158939969971:role/LambdaBasicRole --handler index.handler
