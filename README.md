# Udagram

This application is comprised of a front-end(udagram-frontend) and a backend(udagram-api).
It allows you to register/login and post images with a captions that was provided by udacity.

The idea of the project is to use AWS services to deploy a full-stack app and maintain it with CircleCi CI/CD.

Live application: [Click Here](http://udagrambucket112.s3-website-us-east-1.amazonaws.com)

### Application dependencies
- Node

### AWS infrastructure
- An RDS database running Postgres for user and post storage.
- An S3 bucket for hosting the frontend application(udagram-frontend) and uploaded of images.
- Elastic Beanstalk environment with node for the API(udagram-api) server.

### CircleCI pipeline process
 1. Alteration to the code is committed and pushed to GitHub.
 2. CircleCI picks up the event getting triggered and runs jobs specified in the .circleci/config.yml.
 3. The final step in the job is to upload the latest version of the build to AWS(S3/EB).

Udagram build status 

[![Yfelipe](https://circleci.com/gh/Yfelipe/udagram-aws.svg?style=shield)](<LINK>)

### Documents
In the docs folder you can find a architecture diagram of the application flow and a deployment CI/CD diagram.  
