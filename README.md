# CLI

# Elastic Beanstalk.
eb config save Springapp1-env --cfg devops    
eb config get our-env-test-config

All at once
Rolling
Rolling with additional batch
Blue/Green


# ECS
Fargate want your container to share resources	

# KMS
4KB

# Beanstalk
Share configuration
download configuration -> upload S3

# EC2
Metric scaling
ASGAverageCPUUtilization - This is a predefined metric for target tracking scaling policy. This represents the Average CPU utilization of the Auto Scaling group.

ASGAverageNetworkOut - This is a predefined metric for target tracking scaling policy. This represents the Average number of bytes sent out on all network interfaces by the Auto Scaling group.

ALBRequestCountPerTarget - This is a predefined metric for target tracking scaling policy. This represents the Number of requests completed per target in an Application Load Balancer target group.



# AssumeRole API call

# SQS
Use ChangeMessageVisibility action to extend a message's visibility timeout


# EBS 
An EBS Volume in us-east-1a cannot be attached to us-east-1b
To move a volume across, you first need to snapshot it
EBS can be attached to only one instance at a time
snapshot multiple AZ

# S3
Object Values are the content of the body:
Max Size is 5TB
If uploading more than 100MB , must use “multi-part upload
