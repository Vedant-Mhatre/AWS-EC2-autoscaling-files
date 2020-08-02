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

## --policy-type (string):

One of the following policy types:

* TargetTrackingScaling
* StepScaling
* SimpleScaling (default)

## --adjustment-type (string):

Specifies how the scaling adjustment is interpreted (for example, an absolute number or a percentage). The valid values are ChangeInCapacity , ExactCapacity , and PercentChangeInCapacity.

Required if the policy type is StepScaling or SimpleScaling.

## --scaling-adjustment (integer):

The amount by which to scale, based on the specified adjustment type. A positive value adds to the current capacity while a negative number removes from the current capacity. For exact capacity, you must specify a positive value.

Required if the policy type is SimpleScaling . (Not used with any other policy type.)

## --cooldown (integer)

The duration of the policy's cooldown period, in seconds. When a cooldown period is specified here, it overrides the default cooldown period defined for the Auto Scaling group.

Valid only if the policy type is SimpleScaling.

