# awk
 **_awk_** is text-processing command used to analyze,filter and manipulate structured data such as logs, CSV files and command output.
## Basic syntax 
```
awk [option] 'pattern {action}' input-file > output.file
```

```
df -h | awk 'NR>1 {print $1,$5}'
```
