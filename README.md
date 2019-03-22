# aws-cis-cfn-template
Set up all metric filters and alarms recommended by the CIS Amazon Web Services Foundation.  
This template is a modified from AWS original version. [CloudWatch_Alarms_for_CloudTrail_API_Activity.json](https://s3-us-west-2.amazonaws.com/awscloudtrail/cloudwatch-alarms-for-cloudtrail-api-activity/CloudWatch_Alarms_for_CloudTrail_API_Activity.json)

Added some alarm rules that are not included in the original template.

* 3.2 - Ensure a log metric filter and alarm exist for Management Console sign-in without MFA
* 3.3 - Ensure a log metric filter and alarm exist for usage of "root" account
* 3,7 - Ensure a log metric filter and alarm exist for disabling or scheduled deletion of customer created CMKs
* 3.8 - Ensure a log metric filter and alarm exist for S3 bucket policy changes
* 3.9 - Ensure a log metric filter and alarm exist for AWS Config configuration changes

Following rules included in the original version are not included.

* EC2InstanceChanges
* EC2LargeInstanceChanges

## Reference
**Creating CloudWatch Alarms with an AWS CloudFormation Template**  
https://docs.aws.amazon.com/awscloudtrail/latest/userguide/use-cloudformation-template-to-create-cloudwatch-alarms.html
