```
aws ec2 create-launch-template \
    --launch-template-name autoscaletemplate \
    --version-description version1 \
    --tag-specifications 'ResourceType=launch-template,Tags=[{Key=purpose,Value=production}]' \
    --launch-template-data file://template-data.json
```

## aws ec2 create-launch-template

--launch-template-data
(Mandatory)ImageId
(Mandatory)InstanceType



AWS original documentation:https://docs.aws.amazon.com/autoscaling/ec2/userguide/create-launch-template.html#create-launch-template-aws-cli
