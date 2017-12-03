# College Bebop

In a lot of ways, going to college is a lot like being on the crew of the 

This app will tell you your future. Or, what your future might look like. Or what someone else's future might look like.

## Where to Find the Thing Online


## Roll Your Own Setup and Deploy

This is the slightly more complicated, but slightly more fun way of doing things. There are two major steps to it: configuring your AWS credentials and then configuring the app environment.

All of the following instructions were designed for MacOS 10.13 (High Sierra).

### AWS Credentials

1. Install the AWS CLI.
2. Set up an IAM user profile to use with the application. You can use your own credentials, or use the AWS IAM console to create a new user. I recommend setting up a user called `serverless`.
3. Once you've decided which to use, make sure you set up your profile using the AWS CLI. You can see the profiles you've set up locally by running `cat ~/.aws/credentials`. You should see the profile name you've configured in brackets (i.e., `[profilename]`). Remember this, because that will be the one you're going to use.

### Configuring Your Environment

1. Install Node.js 6.10.3. This is the latest version supported by AWS Lambda. I like to use NVM to manage my Node versions.
2. Install serverless (`npm install -g serverless`).
3. Install Yarn. On a Mac, Homebrew is a good option (`brew install yarn` or, if you use NVM, `brew install yarn --without-node` so that it will default to the Node version specified by your `.nvmrc` file.