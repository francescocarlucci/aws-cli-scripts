# AWS CLI Scripts

A collection of scripts and commands to use with AWS CLI

### Basic

- aws configure

### CloudWatch

- aws logs describe-log-groups
- aws logs delete-log-group --log-group-name /aws/lambda/hello-node

### Lambda

- aws lambda list-functions
- aws lambda list-functions | grep FunctionArn | cut -d '"' -f 4
- aws lambda list-functions | grep FunctionName | cut -d '"' -f 4
- aws lambda create-function --function-name hello-node --zip-file fileb://function.zip --runtime nodejs14.x --role arn:aws:iam::158939969971:role/LambdaBasicRole --handler index.handler
- aws lambda update-function-code --function-name hello-node --zip-file fileb://function.zip
- aws lambda delete-function --function-name hello-node
