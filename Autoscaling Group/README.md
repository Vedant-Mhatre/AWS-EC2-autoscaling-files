  ```
  aws autoscaling create-auto-scaling-group && \
    --auto-scaling-group-name lab-as-group && \
    --launch-configuration-name lab-lc && \
    --load-balancer-names LOADBALANCERNAME && \
    --max-size 4 && \
    --min-size 2 && \
    --vpc-zone-identifier SUBNET1,SUBNET2
  ```
  
## aws autoscaling create-auto-scaling-group
  
'*' mandatory
  ## options:

## --auto-scaling-group-name * (string):

The name of the Auto Scaling group, minimum length 1


## --max-size * (integer):

The maximum size of the group.

## --min-size * (integer):

The minimum size of the group.

## --vpc-zone-identifier

A comma-separated list of subnet IDs for your virtual private cloud (VPC).

Replace LOADBALANCERNAME and SUBNET with your data

AWS Autoscaling Group official documentation:

https://docs.aws.amazon.com/autoscaling/ec2/APIReference/API_CreateAutoScalingGroup.html
