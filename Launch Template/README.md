```
aws ec2 create-launch-template \
    --launch-template-name autoscaletemplate \
    --version-description version1 \
    --launch-template-data '{"NetworkInterfaces":[{"DeviceIndex":0,"AssociatePublicIpAddress":true,"Groups":["sg-7c227019"],"DeleteOnTermination":true}],"ImageId":"ami-01e24be29428c15b2","InstanceType":"t2.micro","TagSpecifications": [{"ResourceType":"instance","Tags":[{"Key":"purpose","Value":"webserver"}]}]}'
```

## aws ec2 create-launch-template

## --launch-template-data

ImageId: Id of AMI from which to launch instances
InstanceType 
(Optional) Storage and Network settings


AWS original documentation:https://docs.aws.amazon.com/autoscaling/ec2/userguide/create-launch-template.html#create-launch-template-aws-cli
