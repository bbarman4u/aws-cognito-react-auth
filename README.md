## Getting Started

## Pre-requisites
- Install Nodejs 14.x+ required for latest version of AWS Amplify SDK.
  - Install on MacOS or Linux using NVM. Instructions [here](https://github.com/nvm-sh/nvm#installing-and-updating)
  - Install on Windows using NVM for Windows. Instructions [here](https://learn.microsoft.com/en-us/windows/dev-environment/javascript/nodejs-on-windows)
- Install yarn
  - `npm install -g yarn`

- Create the Cognito User Pool in your AWS Account.
#### Install dependencies

run `yarn` in the root directory

#### Change configuration to add AWS cognito specific details

- Create a `.env` file at the root of the project folder
- Populate the following keys with the respective values about your cognito pool
```
REACT_APP_REGION=<Enter AWS region>
REACT_APP_USER_POOL_ID=<Enter cognito pool id >
REACT_APP_USER_CLIENT_ID=<Enter cognito app client id>

```

#### Start the app

run `yarn start` in the root directory

#### Build the app (for production)

run `yarn build` in the root directory

## About AWS Cognito

AWS Cognito is a managed authentication service by AWS. To use it's APIs we use [AWS Amplify SDK](https://docs.amplify.aws/lib/auth/getting-started/q/platform/js#create-authentication-service). AWS Amplify is the AWS counterpart of Google's Firebase.

## Upgrading Yarn
### Using Yarn for upgrading the aws-amplify

`yarn upgrade --latest --pattern aws-amplify`
