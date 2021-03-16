# Pipeline

[The circle ci page is here](https://app.circleci.com/pipelines/github/frank3stein/fullstackjs-deployment)

The pipeline builds the backend and frontend simultaneously. Then

- It lints and tests the frontend, if it passess the tests
- It deploys frontend to an s3 bucket (only if the commit is on master branch) and 
- It deploys the backend to an ElasticBeanstalk environment.