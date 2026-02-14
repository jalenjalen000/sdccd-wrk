# Python variables

Variables are human-friendly names of memory locations

## Objective

1. Understand how to define variables in Python.
2. Gain a clear understanding of how the Python interpreter allocates memory addresses to variables.
3. Skilled in troubleshooting techniques.

## Prerequisite

- Python literals lecture & lab
- Programming variables lecture

## What do you need to complete this exercise?

- Please follow my video tutorial [installing Python and PyCharm CE on Windows](https://youtu.be/nFN0JW43GKY). Note: The version you see may differ slightly from what is shown in the video.
- Use the PyCharm IDE to write and compile your code. Submit your responses in a Markdown file on GitHub. Ensure that all code included in the Markdown file runs without errors. Refer to [Submitting Your Assignment Using GitHub](https://sdccd-edu.zoom.us/rec/share/F4rK6ZABMXlRn4aGlZ9P005e-iRKwq8rr9KuawDoJ77TdkybKU2tpf4l4QSe113g.ut4jpVaqaPY0oI7b?startTime=1725121532000) for detailed instructions.

### Variable definition

No need to declare the variable data type; variables can be assigned values or strings as needed.

```
<class 'int'>
<class 'float'>
1000.0
Hello World
Single quote can also be used
```

### Variable memory usage

```
var1 = 10
```

```
# Check the memory address of var1 by using the following statement
print(hex(id(var1)))
```

```
var1 = 100
# Check the memory address of var1 again
```

```
var1 = 10
print (hex(id(var1)))
var1 = 100
print (hex(id(var1)))
```

You should see two distinct addresses for var1. Explain why there are two different addresses and what happened to the first one.

Unlike C++, Python stores a certain value under one address the first time it's defined. var1's value changed from 10 to 100, so that 100 was assigned a new address upon creation. Any other variables equal to 10 will take take the first address.

```
var2 = 100
print (hex(id(var2)))

# Check the memory address of var2. Did the Python interpreter assign a new memory address or reuse the existing one?

The interpreter used the same address as var1.
```

```
# Write your code here
```

### Memory map

```
str1 = "Hello"
str2 = "World"
```

```
# Find out the memory addresses of each character in str1 and str2.
# The following is the example
```

```
print(hex(id(str1[0])), hex(id(str1[1])))  # where 0 is the first index and 1 is the second index
# Use the same method as described above to find the addresses of additional characters and complete the table below.
```

| Address in hexadecimal | Char |
| #0x7ffbfd155448           H           
| #0x7ffbfd1559b8           E         
| #0x7ffbfd155b08           L         
| #0x7ffbfd155b08           L          
| #0x7ffbfd155b98           O           
| #0x7ffbfd155718           W          
| #0x7ffbfd155b98           O          
| #0x7ffbfd155c28           R         
| #0x7ffbfd155b08           L         
| #0x7ffbfd155988           D           

### Problem-solving

Let the variable `x` be `dog` and the variable `y` be `cat`. Write the values returned by the following operations: **Try solving without writing in Python.**

- x + y
- "the " + x + " chases the " + y
- x * 4

dogcat
the dog chases the cat
dogdogdogdog

If `x = 50`. Use an assignment statement to increment the value of `x` by 1.

```
# x + 1

```

### Troubleshooting

Please troubleshoot the following issue **without using Python**, and explain your reasoning.

a. `hello = "hello"`
b. `_var = 100`
c. `!var_1 = 200`
d. `print = "print me"`
e. `False = 0`

a. hello = "hello"
This is okay because quotes are used correctly and a string can have the same contents as its name.
b. _var = 100
Still works because string names can use underscores. It's a number, so no need for quotes.
c. var_1 = 200
Exclamation points can't be used. Only underscores, numbers and letters.
d. print1 = "print me"
Destroys the native "print" function if you redefine it.
e. false = 0 
You can't use "False" as a variable name. It's an existing keyword that cannot be altered.

## Challenges

Please describe the challenges you faced during the exercise.

```python
# Memorizing the statement for returning an address. It's a little complicated at first glance.
# I forgot a few rules for variable definitions.

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

```

**End of exercise**
