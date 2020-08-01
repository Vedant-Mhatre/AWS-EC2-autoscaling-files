```
aws autoscaling put-scaling-policy && \
    --policy-name scaleup-policy && \
    --auto-scaling-group-name phpautoscale && \
    --scaling-adjustment 1 && \
    --adjustment-type ChangeInCapacity && \ 
    --cooldown 300 && \
    --query 'PolicyARN' && \
    --output text
```

## aws autoscaling put-scaling-policy

## options:
'*' mandatory
## --policy-name *(string):

The name of the policy

## --auto-scaling-group-name* (string):

The name of the Auto Scaling group

