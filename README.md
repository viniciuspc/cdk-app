# CDK JavaScript project Example

This example we will use AWS CDK to create an APP to trigger a lambda function when a image to a S3 bucket, this lambda function will them run the AWS Reckoginition service in this image and store the results in an DynamoDB table

This example will generate the following resources:
* A S3 Bucket to upload and store images´
* A lambda function to use AWS Reckoinition and store the results in a DynamoDB table
* A DynamoDB table to store the result
* The required IAM Roles for the services.

The `cdk.json` file tells the CDK Toolkit how to execute your app. The build step is not required when using JavaScript.

Edit the `bin/cdk-app.js` to change the account and region to deploy the app. If not specified it will use the current aws-cli configuration.

## Steps to deploy
* `npm install` to install dependecies
* `cdk bootstrap`
* `cdk deploy`
If want to destroy all the resources:
* Make sure to delete all the images store in the S3 Bucket
* `cdk destroy`

## Useful commands

* `npm run test`         perform the jest unit tests
* `cdk bootstrap`        to bootrap the application
* `cdk deploy`           deploy this stack to your default AWS account/region
* `cdk diff`             compare deployed stack with current state
* `cdk synth`            emits the synthesized CloudFormation template
* `cdk destroy`          to destroy the application
