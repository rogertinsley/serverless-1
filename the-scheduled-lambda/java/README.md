# The Scheduled Lambda

This is an example CDK stack demonstrating how to use AWS EventBridge to invoke a Lambda function on a schedule or using a cron expression. The Lambda function will then write the request ID to a DynamoDB table.

![The Scheduled Lambda Architecture Diagram](img/the-scheduled-lambda.png)

**WARNING**: By default the EventBridge rule has been configured with a rate of 2 minutes, so you are able to quickly see the result of this example. I would strongly recommend destroying the stack using `cdk destroy TheScheduledLambdaStack` so that the scheduled run does not lead to AWS billing you for function invocations.

More information on schedule expressions for AWS EventBridge to change the run frequency of this project can be found [here](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html).

## Useful commands

 * `mvn package`     compile and run tests
 * `cdk ls`          list all stacks in the app
 * `cdk synth`       emits the synthesized CloudFormation template
 * `cdk deploy`      deploy this stack to your default AWS account/region
 * `cdk diff`        compare deployed stack with current state
 * `cdk docs`        open CDK documentation

Enjoy!
