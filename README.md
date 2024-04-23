# zenclass-task6
devops zen classes - Syntax for all loops in shell scripting
### 1. for Loop:
```hcl
for variable in value1 value2 ... valuen
do
    # Commands to execute for each value
done
```
### Example 
```hcl
for i in {1..5}
do
    echo "Value: $i"
done
```
### 2. while Loop:
```hcl
while [ condition ]
do
    # Commands to execute as long as condition is true
done
```
### Example
```hcl
count=0
while [ $count -lt 5 ]
do
    echo "Count: $count"
    ((count++))
done
```
### 3. until Loop:
```hcl
until [ condition ]
do
    # Commands to execute as long as condition is false
done
```
### Example 
```hcl
count=0
until [ $count -eq 5 ]
do
    echo "Count: $count"
    ((count++))
done
```
In these examples:

'variable', 'condition', 'value1', 'value2', etc., are placeholders and should be replaced with appropriate variable names, conditions, or values according to your script's requirements.
'[ condition ]' denotes a conditional expression enclosed within square brackets. You can use various comparison operators like -eq (equal), -ne (not equal), -lt (less than), -gt (greater than), -le (less than or equal to), -ge (greater than or equal to), etc.
