# lambda-function-notified-sns-subscription
## This Lambda function has been listen to Cloudwatch log group for another Lambda function when another Lambda function run primary Lambda function has been listen to Cloudwatch log group and gets and notified-sns-subscription
---
# Create Policies for granting Role permission to Access Resources Go to `Identity and Access Management (IAM)` and create Policies


## cloudwatch Access Policy

```json
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "VisualEditor0",
            "Effect": "Allow",
            "Action": "cloudwatch:*",
            "Resource": "*"
        }
    ]
}
```

## Create Role by previous Policies for granting Lambda permission to Access Resources make sure about role type `AWS service` and Common use cases for `Lambda` let's Create Function don't forget used Created Role for Lambda

---

## Add `environment variable` with `key` name  `SNS_TOPIC_ARN` and mention  `Amazon Resource Names (ARN)` of `Topic` or `subscription` we are Created you can Find it with Specific Topic Details via `Amazon SNS` Console


![Items.png](/Items.png)



## Make Sure `add trigger` From `Function overview` Trigger configuration add a `CloudWatch Logs` as Source Please select the CloudWatch Logs log group that serves as the event source. Log Events sent to the log group will trigger your Lambda function with the contents of the logs received.


![Items2.png](/Items2.png)
