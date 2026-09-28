# AWS_CloudWatch_Alarms

# AWS CloudWatch Alarms Assignment

## Module 3 – CloudWatch Alarms

### Project Overview

This assignment demonstrates how to monitor AWS resources using Amazon CloudWatch Alarms. It includes monitoring estimated AWS billing charges and EC2 CPU utilization, with email notifications through Amazon SNS.

### Objectives

* Monitor estimated AWS charges.
* Create a billing alarm when charges exceed $500.
* Monitor EC2 instance CPU utilization.
* Create an alarm when CPU utilization exceeds 65%.
* Configure SNS email notifications for alarm states.

### AWS Services Used

1. **Amazon CloudWatch** – Monitors AWS metrics and triggers alarms.
2. **Amazon EC2** – Provides the virtual machine whose CPU utilization is monitored.
3. **Amazon SNS** – Sends email notifications when alarm thresholds are crossed.

### Task 1: Billing Alarm

| Configuration | Value             |
| ------------- | ----------------- |
| Alarm Name    | Billing-Alarm-500 |
| Metric        | EstimatedCharges  |
| Currency      | USD               |
| Statistic     | Maximum           |
| Period        | 6 Hours           |
| Threshold     | Greater than $500 |
| Alarm State   | In alarm          |
| Notification  | Amazon SNS        |

**Result:** Created a CloudWatch billing alarm to monitor estimated AWS charges above $500.

### Task 2: EC2 CPU Utilization Alarm

| Configuration | Value                |
| ------------- | -------------------- |
| Alarm Name    | EC2-CPU-Alarm-65     |
| Metric        | CPUUtilization       |
| Statistic     | Average              |
| Period        | 5 Minutes            |
| Threshold     | Greater than 65%     |
| Evaluation    | 1 out of 1 datapoint |
| Notification  | Amazon SNS           |

**Result:** Created a CloudWatch alarm to monitor EC2 CPU utilization above 65%.

### SNS Email Notification

An Amazon SNS topic was configured to send email notifications when an alarm enters the ALARM state. The email subscription must be confirmed to receive notifications.

### Conclusion

Successfully created two Amazon CloudWatch alarms to monitor AWS billing charges and EC2 CPU utilization. Configured Amazon SNS for email notifications to support monitoring and alerting.

### Screenshots

The final CloudWatch screenshot showing both created alarms is included as assignment evidence.

### Author

Dharshan K R

### Course

Intellipaat – AWS Cloud Computing

### Module

Module 3 – CloudWatch Alarms Assignment

