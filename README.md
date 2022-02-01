# PYTHON-FOR-DATA-SCIENCE
complete coding and documentation for python and datascience.

# CONTROL FLOW
```
- if
- if else
- while
- do while
```

## Python if

if is a decision  making statement,if the condition is true then the certain block will be executes otherwise the else block will be executed.

### Syntax:

```
if(condition):
  <block of statement>
else:
  <block of statement>
```
### Example

```
age = 22;
if age>18:
  print("you are eligible for voting")
else:
  print("ypu are not eligible for voting")
```

## Python if else if

if else if is the alternate statement of if,means the ``if`` condition is false then the ``else if`` condition is will be executed and both the blocks are false then the else part will be executed.

### Syntax:
```
if(condition):
  <block of statement>
else if (condition):
  <block of statement>
else:
<block of statement>

```

### Example
```
age = 22;
if age>18 and age<22:
  print("you are eligible for voting")
else if age>18 and age>22:
  print("you are eligible for president election voting)
else:
  print("ypu are not eligible for voting")
```

## Nested if Statement
A nested if is an if statement that is the target of another if statement.Nested if statement means if statement inside another if statement.

### Syntax:

```
if(condition 1):
  <Block of statement>
  #Executes when condition 1 is true
  if(condition 2):
    <Block of statement>
    #Executes when condition 2 is true
  #if Block ends here
#if Block ends here    

```

### Example

```
