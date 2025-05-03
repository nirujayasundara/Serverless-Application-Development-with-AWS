# Serverless-Application-Development-with-AWS
This application showcases the power of serverless architecture using AWS Lambda (Node.js), DynamoDB, and API Gateway. The serverless approach allows for scalable and cost-efficient backend development without managing traditional servers.
omponents and Workflow
User Interaction

The user interacts with the application through a web interface. Requests are made to the /views endpoint.
Amazon API Gateway

API Gateway serves as the entry point for all client requests. It provides RESTful API endpoints that trigger AWS Lambda functions.
AWS Lambda Function (Node.js)

The Lambda function, written in Node.js, processes the incoming requests. It performs various operations, such as reading and writing data to/from DynamoDB.
Amazon DynamoDB

DynamoDB is a fully managed NoSQL database service used to store and retrieve application data. The Lambda function interacts with the DynamoDB table to perform CRUD operations.
Static Content Hosting on Amazon S3

The static web content, including HTML, CSS, and JavaScript files, is hosted on Amazon S3. The JS script handles fetching data from the API and uploading files to S3.
JavaScript Script

The JS script running on the client side interacts with the API Gateway to fetch data and uploads files to S3.

Steps to Setup

1. Create a DynamoDB Table
   
1.Go to the Amazon DynamoDB Console.
2.Click on "Create table."
3.For Table name, enter cloud_resume-test.
4.For Partition key, enter id (Number).
5.Click "Create table."
6.Add an item to your table with the following attributes:
    id: 0
  views: 0

2. Create a Lambda Function
