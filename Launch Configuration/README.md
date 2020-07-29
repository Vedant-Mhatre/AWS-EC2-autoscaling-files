```
aws autoscaling create-launch-configuration --image-id AMIID --instance-type t2.micro --key-name KEYNAME --security-groups SECURITYGROUPID --user-data --launch-configuration-name autoscaleconfig
```

--image-id (string):

The ID of the Amazon Machine Image (AMI) that was assigned during registration.

--security-groups (list):

A list that contains the security groups to assign to the instances in the Auto Scaling group.

--user-data (string):

The Base64-encoded user data to make available to the launched EC2 instances.

--launch-configuration-name (string)

The name of the launch configuration.So is this case, the name "autoscaleconfig" will be given to the launch configuration

Replace AMIID, KEYNAME, SECURITYGROUPID with your data.

AWS Launch configuration official documentation:
https://docs.aws.amazon.com/cli/latest/reference/autoscaling/create-launch-configuration.html
