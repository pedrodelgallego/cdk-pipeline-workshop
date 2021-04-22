## Getting started with CDK pipelines

In this chapter we will create a Continuous Deployment (CD) pipeline for the app developed in previous chapters.

CD is an important component to most web project, but can be challenging to set up with all the moving parts required. The CDK Pipelines construct makes that proccess easy and streamlined from within your existing CDK infrastructure design.

These pipelines consist of “stages” that represent the phases of your deployment process from how the source code is managed, to how the fully built artifacts are deployed.

## Create Pipeline Stack
The first step is to create the stack that will contain our pipeline. Since this is separate from our actual “production” application, we want this to be entirely self-contained.

Create a new file under lib called ```lib/pipeline-stack.ts``` Add the following to that file. 

```ts
import * as cdk from '@aws-cdk/core';

export class WorkshopPipelineStack extends cdk.Stack {
    constructor(scope: cdk.Construct, id: string, props?: cdk.StackProps) {
        super(scope, id, props);

        // Pipeline code goes here
    }
}
```