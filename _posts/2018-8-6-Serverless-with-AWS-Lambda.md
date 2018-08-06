---
layout: post
title: Serverless with AWS Lambda
---


AWS Lambda is a service that reduces the amount of backend work for your app. This allows engineering teams to run code without provisioning or managing servers. You just upload your code and Lambda will take care of everything required to run and scale your code.

### Why this matters

As an example, when an event happens, Lambda will spin up, execute, respond, and then spin down. AWS Lambda is essentially cutting out the need for the server to be up 24 hours a day.

That is incredible!! This will allow engineering teams to **iterate faster**, **increase innovation**, and **reduce their overhead**.

### Getting started

You must have an [AWS account](https://aws.amazon.com/free/) for this to work. Don't worry, its **free**! After you have an account, you need to make a new user. Video instructions here: [Creating AWS Access Keys](https://www.youtube.com/watch?v=HSd9uYj2LJA).

### Enter Serverless

[Serverless](https://serverless.com/) is a framework that uses cloud services (like AWS Lambda) to operationalize a server less framework. In my opinion they make getting started with AWS Lambda more straightforward.

1. [Install Serverless](https://serverless.com/framework/docs/getting-started/) globally on your machine
2. [Set up AWS credentials with Serverless](https://serverless.com/framework/docs/providers/aws/guide/credentials/)
3. [Create a service](https://serverless.com/framework/docs/providers/aws/cli-reference/create/)

In the working directory of your project you will need to create a service. If you are using `Node.js` you can create a template that will create a service with the proper file structure to build, test, and deploy a Lambda function to AWS. That might look like this:

```
$ mkdir restapi-example && cd restapi-example

$ serverless create --template aws-nodejs
```

Before deploying, make sure to [define your functions](https://serverless.com/framework/docs/providers/aws/guide/functions/) and routes.

### Deploying to AWS

Now, deploy your function:

```
sls deploy
```

If your deploy is successful you should see a screen like this in your terminal:

![an image alt text]({{ site.baseurl }}/images/sls-deploy.png "terminal sls deploy")

The output should show you all of the functions you have defined and the public routes where you can access the functions. You can test your deployment in the browser or by running cURL from the terminal:

```
$ curl https://yf9ut0kdr1.execute-api.us-east-1.amazonaws.com/dev/todo/blog-post-example
```

In my cURL request I passed in a parameter called **"blog-post-example"**.

Within **AWS CloudWatch** you are immediately able to inspect and analyze the event.

![an image alt text]({{ site.baseurl }}/images/aws-cloudwatch.png "aws-cloudwatch-logs")


**Congratulations!** Your AWS Lambda functions are live!

It's fun to get a simple endpoint live and it is the foundation to building more valuable applications.

Were you able to deploy successfully? If not, feel free to reach out with any questions. I regularly work with customers and engineers to remove their technical hurdles 🙂
