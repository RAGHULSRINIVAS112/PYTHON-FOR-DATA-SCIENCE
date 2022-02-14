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

## Python elif

if else if or elif is the alternate statement of if,means the ``if`` condition is false then the ``else if`` condition is will be executed and both the blocks are false then the else part will be executed.

### Syntax:
```
if(condition):
  <block of statement>
elif (condition):
  <block of statement>
else:
<block of statement>

```

### Example
```
age = 22;
if age>18 and age<22:
  print("you are eligible for voting")
elif age>18 and age>22:
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
i=int(input("Enter a number"))

if i<=10:
  print("i is less than 10")
  if i<15:
    print("i is less than 15")

  if i<12:
    print("i is less than 12")

else:
  print("i is greater than 15")
  
```


# FUNCTIONS

Functions is the Block of code runs when it is called.The main idea of functions is to the same block of code that need to repeated in some conditions so if the repeated code is declared as a function then it can be used wherever by calling that function.

## Creating the function

you can create the function by using ``def`` keyword before the function name.

### Syntax:

```
def <function name>:
  <Block of code>
```

### Example:

```
def name:
  print("Raghul")
  
```

## Calling the function
you can call the function by writting the function name and paranthesis containg perameters if we want.

### Example

```
def name():
print("Raghul")

name()

```
### Output

```
Raghul
```

## Arguments

Arguments are the value passed inside pranthesis of the function.we can pass multiple values inside the pranthesis by seperating by commas``,``.

### Example:

```
def hello_name(name):
  print(f'hello {name}')

hello_name("Raghul")
```
### Output:
```
Hello Raghul
```
### Default Arguments

Default arguments are the placeholder or default value for the values inside the functions.If the called function does not have any value then the default argumets will be passed.

### Example:
```
def hello_name(name):
  print(f'hello {name}')

hello_name()
```
### Output:
```
TypeError                                 Traceback (most recent call last)

<ipython-input-30-1817a56c09c3> in <module>()
      2   print(f'hello {name}')
      3 
----> 4 hello_name()

TypeError: hello_name() missing 1 required positional argument: 'name'
```

In the above Example if we call the function with no arguments it will show error show we we will use default arguments



### Example:
```
def hello_name(name="Meow"):
  print(f'hello {name}')

hello_name()
```
### Output:
```
hello Meow
```
Here ```Meow``` is the default argument.


### Return Statement

Return Statement is the statements exits the function and goes back to the function call executes the return value or expression.
The return statement can store the values in the function call by creating the variables but the other methods cannot.

```
def print_result(a,b):
  print(a+b)
  
result=print_result(10,20)

print(result)
```
### Output:
```
#This output is for line no 203
30
None
```
Here it display ``None`` value for calling the result variable in this case we use ```return``` keyword it allows the user to store the values in the function call with a variables.

### Example:

```
def print_result(a,b):
  return(a+b)
  
result=print_result(10,20)

print(result)
```
### Output:

```
30
```
In this Example the output is ``30`` because in return statement the function call statement stored in the variable called ``result`` will be displayed if the variable is called.

## Arbitary Arguments(Args)

Arbitary arguments are also called args. arbitary arguments are used to add n number of arguments without predefine parameters.args form the set of values as tuple in the function.

### Example:

```
def func(*args):
  print('the number belonmgs to index zero is {}'.format(*args[0]))


func('1','2');
```

### Output:

```
the number belonmgs to index zero is 1
```
## Keyword arguments 

Keyoword arguments are also called as kwargs.keyword arguments are use to add n number of dictonaries wothout defining parameter.

### Example:
```
def funct(**kwargs):
  if 'fruit'in kwargs:
    print('my fruit of choice {}'.format(kwargs['fruit']))

funct(fruit="apple")
```
### Output:
```
my fruit of choice apple
```

