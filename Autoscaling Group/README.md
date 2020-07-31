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
  
  ## options:
