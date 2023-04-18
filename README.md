## Getting Started

#### Install dependencies

run `yarn` in the root directory

#### Change configuration to add AWS cognito specific details

- Create a `.env` file at the root of the project folder
- Populate the following keys with the respective values
```
REACT_APP_REGION=<Enter AWS region>
REACT_APP_USER_POOL_ID=<Enter cognito pool id >
REACT_APP_USER_CLIENT_ID=<Enter cognito app client id>

```

You can get the required info from you user pool. If you don't know how to setup aws cognito then please [read this first](https://dev.to/mubbashir10/implement-auth-in-react-easily-using-aws-cognito-5bhi)

#### Start the app

run `yarn start` in the root directory

#### Build the app (for production)

run `yarn build` in the root directory

## About AWS Cognito

AWS Cognito is a managed authentication service by AWS. To use it's APIs we use [AWS Amplify SDK](https://docs.amplify.aws/lib/auth/getting-started/q/platform/js#create-authentication-service). AWS Amplify is the AWS counterpart of Google's Firebase.

# Using YARN for upgrading the aws-amplify

yarn upgrade --latest --pattern aws-amplify
