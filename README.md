# aws-appsync-demo

AWS Appsync Demo is small project to install and test AWS Appsync to build a small application. You will need a valid AWS account. I am following a video tutorial found in the link below. 

https://www.youtube.com/watch?v=a_klcMRUfaM

Here is a link to additional resources: https://aws.amazon.com/appsync

## Installation
Run the commands below and follow the prompts.
Click this link if you need to install npm: [https://nodejs.org]
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

..*> C:\Users\webberr\aws-appsync-demo>amplify add api
..*> ? Please select from one of the below mentioned services GraphQL
..*> ? Provide API name: awsappsyncdemo
..*> ? Choose an authorization type for the API API key
..*> ? Do you have an annotated GraphQL schema? No
..*> ? Do you want a guided schema creation? true
..*> ? What best describes your project: (Use arrow keys)
..*> ? What best describes your project: Single object with fields (e.g., “Todo” with ID, name, description)
..*> ? Do you want to edit the schema now? (Y/n) Y
..*> ? Do you want to edit the schema now? Yes
..*> Please edit the file in your editor: C:\Users\ryan_\aws-appsync-demo\amplify\backend/api/awsappsyncdemo/schema.graphql
..*> ? Press enter to continue

This will open your editor to modify the GraphQL schema.
