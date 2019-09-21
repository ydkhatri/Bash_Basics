# Loops

There are 3 loops types. They are **while**, **until**, and **for**. **Until** loops very similarly to while loops they are just easier to read in situations than while loops.

## While

The basic syntax for a while loop is:

```Bash
while [ <some test> ]
do
    <commands>
done
```

an example of counting to 10.

```Bash
counter=1
while [ $counter -le 10 ]
do
    echo $counter
    ((counter++))
done
```

## Until

The basic syntax for an until loop is:

```Bash
until [ <some test> ]
do
    <commands>
done
```

the same example of counting to 10.

```Bash
counter=1
until [ $counter -gt 10 ]
do
    echo $counter
    ((counter++))
done
```

### Why use Until

An example of why you would use until:  
Leave the towel on the line until it's dry.

Where using while:
Leave the towel on the line while it is not dry.
Or:
Leave the towel on the line while it is wet.

## For

The basic syntax for a for loop is:

```Bash
for var in <list>
do
    <commands>
done
```

an example with names:

```Bash
names='Stan Kyle Cartman'
for name in $names
do
    echo $name
done
```

### Series

You can process a series of numbers easily by using ```..``` between the first and last number.

Example counting 1 to 10:

```Bash
for value in {1..10}
do
    echo $value
done
```

### Stepping

You can also choose the value to increase or decrease each time and the is called stepping. You add a second ```..``` between the last number in the series and the value, you want to step by.
Example counting down from 10 to 0 by 2.

```Bash
for value in {10..0..2}
do
    echo $value
done
```
