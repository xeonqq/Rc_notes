there is *min_check* (default,1050) and *max_check* (default,1950) in cleanflight. Only if your throttle is below *min_check* and the yaw is larger than *max_check* the vehicle will arm.

## Check Value of *min_check* and *max_check*
- In side cleanflight configurator go to CLI
- for example to increase *min_check* type:
```
get min_check
set min_check=1100 
save
```
- for example to decrease *max_check* type:
```
get max_check
set max_check=1850 
save
```
