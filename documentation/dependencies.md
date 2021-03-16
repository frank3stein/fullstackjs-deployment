# How to Install the Project

* Firstly, clone the project
    - `git clone https://github.com/frank3stein/fullstackjs-deployment.git`

* You can build the frontend and backend by running the commands
    - npm run frontend:build
    - npm run backend:build
    - These commands will run install commands for the each build process as a preprocess.

* Make sure to check if environment variables are configured properly in your environment
    - For backend the environment variables are set at api/src/config/config.ts
    - For frontend the environment variables are set at frontend/src/environments/

* Deploy the project manually
    - npm run frontned:deploy
    - npm run backend:deploy
    - You will need to adjust the elasticbeanstalk config and s3 bucket name in order to configure it for your own AWS account.

* Or deploy the project through CIRCLE CI
    - push the changes to your master branch (makes sure to make the changes described in the manual step, elasticbeanstalk config, s3 bucket name)

[The circle ci page is here](https://app.circleci.com/pipelines/github/frank3stein/fullstackjs-deployment)
