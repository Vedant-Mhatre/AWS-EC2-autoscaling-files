```
aws autoscaling put-scaling policy && \
    --policy-name scaledown-policy && \
    --auto-scaling-group-name phpautoscale&& \
    --scaling-adjustment -1 && \
    --adjustment-type ChangeInCapacity && \
    --cooldown 300 && \
    --query 'PolicyARN' && \
    --output text
```