# Tuples in Python

A tuple in Python is an ordered, immutable sequence of elements. Tuples are defined using parentheses and can contain elements of different data types, including other tuples. Once a tuple is created, its elements cannot be modified, added, or removed. This immutability makes tuples suitable for representing fixed collections of data.

## Objective

- Comprehend the application of tuples
- Understand how a tuple uses a memory
- Apply various operations on tuples

## Prerequisite

- Lists
- Decision and loops
- Input functions
- Python literals
- Programming variables

## What do you need to complete this exercise?

- Please follow my video tutorial [installing Python and PyCharm CE on Windows](https://youtu.be/nFN0JW43GKY). Note: The version you see may differ slightly from what is shown in the video.
- Use the PyCharm IDE to write and compile your code. Submit your responses in a Markdown file on GitHub. Ensure that all code included in the Markdown file runs without errors. Refer to [Submitting Your Assignment Using GitHub](https://sdccd-edu.zoom.us/rec/share/F4rK6ZABMXlRn4aGlZ9P005e-iRKwq8rr9KuawDoJ77TdkybKU2tpf4l4QSe113g.ut4jpVaqaPY0oI7b?startTime=1725121532000) for detailed instructions.

## 1. Exercising tuples

**1a)** Take five inputs from an user and save it in a tuple called `my_tuple`

```
a = input ("Input One:")
b = input ("Input Two:")
c = input ("Input Three:")
d = input ("Input Four:")
e = input ("Input Five:")
my_tuple = (a,b,c,d,e)

```

**1b.** How do you assign a single element in a tuple?

```
single_element_tuple = (1,)
#(I put a comma after the value)
```

**1c.** `my_tuple = (1,2,3,4,3,2,1,2,3,5,4,3,2,1)` Count the repeated integers and print the result on the console.

```
my_tuple = (1,2,3,4,3,2,1,2,3,5,4,3,2,1)
for num in my_tuple:
    print(num, my_tuple.count(num), "repetitions")
```

**1d.** `my_tuple = my_tuple + my_tuple`

Proof that `my_tuple` in part c is different than the `my_tuple` in part d.

```
my_tuple = (1,2,3,4,3,2,1,2,3,5,4,3,2,1)
print(id(my_tuple))
my_tuple = (my_tuple + my_tuple)
print(id(my_tuple))
# (After I changed the tuple on line 3, the address is different when it's printed again.)
```

**1e.** Explain why the following operations aren’t legal for the tuple. Answer without using the Python.

```
x = (1,2,3,4)
x.append(1)
x[1] = "hello"
del x[2]
```
All of these operations are attempts to alter the tuple. They don't work because, unlike lists, you cannot change a tuple after defining it. 

## 2. Packing and unpacking tuples

Python permits tuples to appear on the left side of an assignment operator, in which case variables in the tuple receive the corresponding values from the tuple on the right side of the assignment operator. Here’s a simple example:

```
(one, two, three, four) =  (1, 2, 3, 4)
```

**2a.** What is the data type of each variable?

They are all integers.

**2b.** Python has an extended unpacking feature, allowing an element marked with * to absorb any number of elements not matching the other elements. For example,

```
x = (1, 2, 3, 4)
a, b, *c = x
a, b, c
```

```
(1, 2, [3, 4])
```

**2c.** What will be the result of `a, *b, c = x`?

```
x = (1, 2, 3, 4)
a, *b, c = x
print("a:", a)
print("b:", b)
print("c:", c)

Result:
a: 1
b: [2, 3]
c: 4
```

## 3. Memory management

```
my_x = [100,200,300,400]
my_y = (200,300,400,500)
```

Discuss how memory addresses are assigned to each index of the list and the tuple. Pay attention to new addresses & re-used addresses.

| Index | my_x            | my_x             |
| 0     | 140731780784344 | 140731780787544  |
| 1     | 140731780787544 | 2533184904176    |
| 2     | 2533184904176   | 2533184903792    |
| 3     | 2533184903792   | 2533184903888    |

Numbers appearing in both my_x and my_y are given the same address. 100 and 500 are only used once and not in both the list and tuple, so their addresses only come up once.

## Challenges

Please describe the challenges you faced during the exercise.

```python
# The extended unpacking feature was somewhat confusing.

## Extended unpacking details

Extended unpacking in Python allows you to assign elements from an iterable to variables while using a starred variable (`*`) to capture multiple remaining values. For example:

```python
a, *b = [1, 2, 3, 4]
```

Here, `a` gets `1`, and `b` gets `[2, 3, 4]`. The starred variable always collects the extra elements into a list.

You can also place the star in the middle:

```python
a, *b, c = [1, 2, 3, 4, 5]
```

Now, `a` is `1`, `b` is `[2, 3, 4]`, and `c` is `5`.

Only one starred expression is allowed per unpacking statement. Extended unpacking is useful when working with sequences of variable length while keeping certain positions fixed.


# 

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

# _________________________________________________________________________________________________

```

**End of exercise**
