# aws-appsync-demo

AWS Appsync Demo is small project to install and test AWS Appsync to build a small application. You will need a valid AWS account. I am following a video tutorial found in the link below. 

https://www.youtube.com/watch?v=a_klcMRUfaM

Here are links to additional resources: https://aws.amazon.com/appsync, https://aws-amplify.github.io/docs/

## Getting Started

#### Prerequisites

* [AWS Account](https://aws.amazon.com/mobile/details) with appropriate permissions to create the related resources
* [NodeJS](https://nodejs.org/en/download/) with [NPM](https://docs.npmjs.com/getting-started/installing-node)
* [AWS CLI](http://docs.aws.amazon.com/cli/latest/userguide/installing.html) `(pip install awscli --upgrade --user)`
* [AWS Amplify CLI](https://github.com/aws-amplify/amplify-cli) (configured for a region where [AWS AppSync is available](https://docs.aws.amazon.com/general/latest/gr/rande.html#appsync_region)) `(npm install -g @aws-amplify/cli)`

## Installation
Run the commands below and follow the prompts.
Click this link if you need to install npm: https://nodejs.org
npm install -g @aws-amplify/cli

amplify configure

The AWS console will open. Sign into your account and return to the command line. 

Following the prompts you will be asked to specify an AWS Region. Create a new user for your application. I chose amplify-cli-myregion-user.

This will open the IAM console in the AWS dashboard to add a new user. Accept the defaults clicking next:permisions, next:tags and next:review and then create user.

Copy the access key id and secret access key to the clipboard and paste them in commnand prompt. Next we create a profile.

Now that amplify has been installed and configured create a new React app to interact with the new API. 

create-react-app aws-appsync-demo
cd aws-appsync-demo
amplify init

Follow the prompts to set an editor, framework, type, source directory, build, and app start commands. 
amplify add api

Follow the default prompts. 

Execute the following command to save your API 
amplify push


