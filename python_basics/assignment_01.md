# Assignment #001

**Below are the problem sets for Python Basics.**

## Question 1

In the below elements which of them are values or an expression? 

eg:- 
- values can be integer or string and 
- expressions will be mathematical operators.

```
*
'hello'
-87.8
-
/
+
6
```

#### Solution

|element|value/expression|
|--|--|
|* | expression |
|'hello' | value |
|-87.8 | value |
|-  | expression |
|/ | expression |
| + | expression |
|6| value |

## Question 2

What is the difference between string and variable?

#### Solution

- String: 
  - A string is a collection of characters enclosed within single `'` or `"` quotation marks.
  - String is of Sequence data type.
  - eg.
    ```python
    my_name = "Himanshu"
    print(type(my_name))    # results 'str'
    ```
- Variable:
  - A variable is a name to which any value can be assigned.
  - A variable can be of type integer or string or boolean etc.
  - eg.
    ```python
    """
    `my_name` is variable which holds value `Himanshu` which is of type string.
    """

    my_name = "Himanshu"

    """
    `my_age` is a variable which holds value `26` which is of type int.
    """

    my_age = 26
    ```

## Question 3

Describe three different data types.

#### Solution

- Numeric Data types
  - represents the data that has a numeric value.
  - main numeric data types are,
    - Integers
    - Floating-point
    - Complex Numbers
    - eg.
        ```python
        print(55)       # integer type
        print(-12.231)  # floating point number
        print(complex(2, 2))    # represents (2+2j), complex number
        ```
- Boolean Data type
  - Boolean data type have two values either `True` or `False`.
  - Used to determine whether logic of a comparison is correct.
  - eg.
    ```python
    print(10>9)     # results `True`
    print(99<11)    # results `False`
    ```
- Sequence Data type
  - Sequence data type are collection of similar or different data types values.
  - eg. String, lists etc.
    ```python
    print("Winter Soldier!") # string data type
    ```

## Question 4

What is an expression made up of? What do all expressions do?

#### Solution

Expression is a combination of values, variables, operators or function calls. Expression is something that needs to be evaluated by the interpreter that produces a value.

eg.
```python
pi = 3.14  # this is a statement

print(pi*2)   # this is an expression
```

## Question 5

This assignment statements, like spam = 10. What is the difference between an expression and a statement?

#### Solution

A statement does not yields any value, if we fire up our terminal,

```python
>>> 1+3 # this is expression as it will yield 4 as answer
>>> x = 3 # this is a statement 
```

## Question 6

After running the following code, what does the variable bacon contain?

```
bacon = 22
bacon + 1
```

#### Solution

Result,
```
22
```

## Question 7 

What should the values of the following two terms be?

```python
"spam" + "spamspam"
"spam" * 3
```

#### Solution

Result,
```python
>>>'spamspamspam'
>>>'spamspamspam'
```

## Question 8

Why is `eggs` a valid variable name while `100` is invalid?

#### Solution

In python, there are some rules we need to follow when picking the name for a variable:

- The first character must start with an UPPERCASE or LOWERCASE letter of alphabet or UNDERSCORE(_)
- Rest of the name can consist of UPPERCASE or LOWERCASE letter of alphabet or UNDERSCORE(_) or DIGITS(0-9)
- Spaces are not allowed. Instead, use snake_case to make variable names readable.
- Names are case-sensitive. myworld and myWorld are not the same.
- The name of the variable should be something meaningful that describes the value it holds, instead of being random characters.

Therefore,

`100` is invalid whereas `eggs` is a valid variable name.

## Question 9

What three functions can be used to get the integer, floating-point number, or string version of a value?

#### Solution

This method is know as Explicit Type Conversion.

```python
# string to integer
value = '23'    # string type
int_form = int(value)   # we get an integer type

# string to float
value = '231.21'    # string type
float_form = float(value) # we get float point number

# integer to string
value = 45  # integer type
str_form = str(value)   # we get string data type
```

Note, below are some examples that will throw an error

```python
value = "Hello"
int_form = int(value)   # ERROR

value = "23.11"
int_form = int(value)   # ERROR

value = "'21'"
int_form = int(value)   # ERROR
```

## Question 10

Why does this expression cause an error? How can you fix it?

```python
'I have eaten ' + 99 + ' burritos.'
```

#### Solution

We cannot add a string data type with an integer data type. We need to convert integer to string and then evaluate the expression.


```python
>>> 'I have eaten ' + str(99) + ' burritos.'
```

<hr>