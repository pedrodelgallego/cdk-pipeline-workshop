
## Creating a CDK project
In this chapter we will use ```cdk init``` to create a new AWS CDK TypeScript project.

We will also learn how to use the CDK Toolkit to synthesize an AWS CloudFormation template for the starter app and how to deploy your app into your account.

## Create project directory

Create an empty directory on your system:

```sh
mkdir cdk-simple-pipeline && cd cdk-simple-pipeline
```

### cdk init

We will use cdk init to create a new TypeScript CDK project:

```sh
cdk init --language typescript
```

Output should look like this (you can safely ignore warnings about initialization of a git repository, this probably means you don’t have git installed, which is fine for this workshop):

Output should look like this (you can safely ignore warnings about initialization of a git repository, this probably means you don’t have git installed, which is fine for this workshop):

```sh
# Welcome to your CDK TypeScript project!

This is a blank project for TypeScript development with CDK.

The `cdk.json` file tells the CDK Toolkit how to execute your app.

## Useful commands

 * `npm run build`   compile typescript to js
 * `npm run watch`   watch for changes and compile
 * `npm run test`    perform the jest unit tests
 * `cdk deploy`      deploy this stack to your default AWS account/region
 * `cdk diff`        compare deployed stack with current state
 * `cdk synth`       emits the synthesized CloudFormation template

Executing npm install...
✅ All done!
```

As you can see, it shows us a bunch of useful commands to get us started.
