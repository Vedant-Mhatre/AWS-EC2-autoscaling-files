```
aws ec2 create-launch-template \
    --launch-template-name autoscaletemplate \
    --version-description version1 \
    --launch-template-data file://template-data.json
```

## aws ec2 create-launch-template

## --launch-template-data

ImageId: Id of AMI from which to launch instances
InstanceType 
(Optional) Storage and Network settings


AWS original documentation:https://docs.aws.amazon.com/autoscaling/ec2/userguide/create-launch-template.html#create-launch-template-aws-cli
