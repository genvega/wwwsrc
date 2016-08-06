---
layout: post
title:  "AWS labs's Chalice - deploy serverless python UI"
description: "If you have a python UI application runs on EC2 or any other machine environment, you can eliminate the entire hosting cost in favor of per execution model of AWS Lambda and API gateway."
date:   2016-08-06 17:04:43
keywords: "DevOps, Python, Lambda API Gateway"
comments: true
category: technology
---
<p>
I recently got to play with <a href="https://github.com/awslabs/chalice">Chalice</a> for a dashboard we are building at my client's. It is very promising. One way to think about it is of a bridge between the <a href="https://aws.amazon.com/api-gateway/">AWS API Gateway</a> and the <a href="https://aws.amazon.com/lambda/">AWS Lambda</a> serverless compute environment. 
Chalice is not the only way to integrate an API gateway rest call to the Lambda execute engine, however, it does make things easy for a python flask developer. Programmers need only code in the popular <a href="http://flask.pocoo.org"/>flask microframework</a> using familiar metadata constructs such as <a href="http://flask.pocoo.org/docs/0.11/api/#url-route-registrations">routes</a>. Chalice reads the metadata reflectively and converts those into corresponding API gateway endpoints. 
</p>

<p>Additionally, it wraps the Flask app in order to decode the API gateway request to an http request format that Flask understands. This is huge. It bridges the two architectures API gateway and Lambda in a standard, predictable way. That in a nutshell is Chalice. Additionally, it also has logic to detect any boto3 calls that the flask app makes and generate IAM policy that will satisfy permissions that the flask app needs. That is pretty neat. The place I work, not all developers have access to creating IAM policies - for obvious security reasons. Even if I created a POC using Chalice as it was when I first looked at it, my developers would not be able to use it. So, I made a tweak to Chalice and James over at AWS Labs accepted my <a href="https://github.com/awslabs/chalice/pull/85">github pull request</a>. Pretty awesome. As of version 0.1.0, one can just configure a pre-defined IAM role for Chalice to use instead of trying to create one from scratch. FTW!
</p>

<p>
Head over to the <a href="https://github.com/awslabs/chalice">Chalice github repo</a> to get all the latest code and documentation. 
</p>