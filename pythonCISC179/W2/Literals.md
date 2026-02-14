# Python literals

A literal is data whose values are determined by the literal itself.

## Objective

1. Understand how Python uses literals.
2. Differentiate Integer, Float, Boolean and String data types.
3. Understanding how arithmetic operations are performed and recognizing the precedence of operators.

## Prerequisite

- Python & literals lecture

## What do you need to complete this exercise?

- Please follow my video tutorial [installing Python and PyCharm CE on Windows](https://youtu.be/nFN0JW43GKY). Note: The version you see may differ slightly from what is shown in the video.
- Use the PyCharm IDE to write and compile your code. Submit your responses in a Markdown file on GitHub. Ensure that all code included in the Markdown file runs without errors. Refer to [Submitting Your Assignment Using GitHub](https://sdccd-edu.zoom.us/rec/share/F4rK6ZABMXlRn4aGlZ9P005e-iRKwq8rr9KuawDoJ77TdkybKU2tpf4l4QSe113g.ut4jpVaqaPY0oI7b?startTime=1725121532000) for detailed instructions.

### 1. Literals

What will the output be without using Python? Aim for 80% accuracy.

```python
print(5 + 2 - 2)
# 5
print(5 / 2)
# 2.5
print(6 // 2) # // integer division
# 3
print(2. * 3)
# 6.0
print(2 < 4)
# true
print(2 >= 2)
# true
print("Hello"+"World")
# HelloWorld
print("bla" * 3)
# blablabla
print(2 * 3 ** 3)
# 54
print(5 * 25 // 13 + 100 / 2 % 13 // 2)
# 14.0
print(2 * 3 % 5)
# 1
print((2 % -4), (2 % 4), (2 ** 3 ** 2))
# -2 2 512
```

Please verify using Python to determine if you have achieved at least 80% correct answers.

### 2. Data type

What will the output be without using Python? Aim for 80% accuracy.

```python
type("Hello")
# <class 'str'>
type(1+"2")
# typeError
type(1.)
# <class 'float'>
type('A')
# <class 'str'>
type(500)
# <class 'int'>
type(True)
# <class 'bool'>
type("False")
# <class 'str'>
```

Please verify using Python to determine if you have achieved at least 80% correct answers.

### 3. Operator precedence

a) Write your arithmetic expression that uses at least one operator from each group and prove the operator's precedence. For example ```5 * 25 % 13 + 100 / -2 * 13 // 2 ** 3```

-2 ** 3 * 4 // 3 + 5

1. 2 ** 3 = 8
2. = -8
3. -8 * 4 =-32
4. -32 + 5 = -27
b) What will the output be without using Python after writing your arithmetic expression? Use the table below for your reference.

-6

c) Please verify using Python to determine if you have done it correctly.

| Priority | Operator                                                     | Notes                    |
| :------- | :----------------------------------------------------------- | :----------------------- |
| 1        | `**`                                                         | Right to left evaluation |
| 2        | `+`, `-` (note: unary operators located next to the right of the power operator bind more strongly) | unary                    |
| 3        | `*`, `/`, `//`, `%`                                          | Left to right evaluation |
| 4        | `+`, `-`                                                     | binary                   |

## Challenges

Please describe the challenges you faced during the exercise.

```python

# Attempting math in my head was difficult.

# I mistyped a lot of things in my interpreter and recieved a lot of errors.

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

```

**End of exercise**

