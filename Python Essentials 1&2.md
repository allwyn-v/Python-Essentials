### PYTHON ESSENTIALS

Cisco Skills For All - Python Essentials 1 & 2

### THE VERY FIRST PROGRAM


```python
# The very first program, that is, print("hello, world!") consists of 
# The word - print
# An opening and closing parenthesis
# Quotation marks 
# And a sequence of characters that is to be printed
# More over, the print function is a built-in function, meaning it may come from Python itself!
# In some cases, some functions need to be imported using modules, they may be user-defined functions.


print("Hello, World!")
```

    Hello, World!
    

### FUNCTION ARGUMENTS


```python
# The only argument delivered to the print() function in this example is a string:
print("Hello, World!")
```

    Hello, World!
    

What happens when Python encounters an invocation like this one below?

function_name(argument)

* First, Python checks if the name specified is legal (it browses its internal data in order to find an existing function of the name; if this search fails, Python aborts the code)

* Second, Python checks if the function's requirements for the number of arguments allows you to invoke the function in this way (e.g., if a specific function demands exactly two arguments, any invocation delivering only one argument will be considered erroneous, and will abort the code's execution)

* Third, Python leaves your code for a moment and jumps into the function you want to invoke; of course, it takes your argument(s) too and passes it/them to the function;

* Fourth, the function executes its code, causes the desired effect (if any), evaluates the desired result(s) (if any) and finishes its task;

* Finally, Python returns to your code (to the place just after the invocation) and resumes its execution.
 Any keyword arguments have to be put after the last positional argument.


### KEYWORD ARGUMENTS

- The print() function has two keyword arguments that you can use for your purposes. The first is called end.


```python
print("Hello,", end=" ")
print("World!")

```

    Hello, World!
    

- Another kind of argument the print function takes is the sep. Which separates each arguement passed to the function with the desired character.


```python
print("Hello", "World", sep="~")
print("Hello", "world", sep="\n")
```

    Hello~World
    Hello
    world
    


```python
print("this", "is", "without", "using", "the", "sep", "keyword")
print("this", "is", "with", "the", "sep", "keyword", sep="-")
```

    this is without using the sep keyword
    this-is-with-the-sep-keyword
    

Both keyword arguments may be mixed in one invocation


```python
print("this", "is", sep="-", end="*")
print("the", "new", "world", sep="~")
```

    this-is*the~new~world
    

### SUMMARY
1. The print() function is a built-in function. It prints/outputs a specified message to the screen/console window.

2. Built-in functions, contrary to user-defined functions, are always available and don't have to be imported. Python 3.8 comes with 69 built-in functions. You can find their full list provided in alphabetical order in the Python Standard Library.

3. To call a function (this process is known as function invocation or function call), you need to use the function name followed by parentheses. You can pass arguments into a function by placing them inside the parentheses. You must separate arguments with a comma, e.g., print("Hello,", "world!"). An "empty" print() function outputs an empty line to the screen.

4. Python strings are delimited with quotes, e.g., "I am a string" (double quotes), or 'I am a string, too' (single quotes).

5. Computer programs are collections of instructions. An instruction is a command to perform a specific task when executed, e.g., to print a certain message to the screen.

6. In Python strings the backslash (\) is a special character which announces that the next character has a different meaning, e.g., \n (the newline character) starts a new output line.

7. Positional arguments are the ones whose meaning is dictated by their position, e.g., the second argument is outputted after the first, the third is outputted after the second, etc.

8. Keyword arguments are the ones whose meaning is not dictated by their location, but by a special word (keyword) used to identify them.

9. The end and sep parameters can be used for formatting the output of the print() function. The sep parameter specifies the separator between the outputted arguments, e.g., print("H", "E", "L", "L", "O", sep="-"), whereas the end parameter specifies what to print at the end of the print statement.
### LITERALS

- A literal is data whose values are determined by the literal itself.


### INTEGERS

- Integers are nothing but numeric literals of the type int. These are devoid of the fractional part.
- e.g., 2,3,54,55
- Since python doesn't allow whitespaces between any characters or numbers, in order to separate large numbers we can use underscores or simply without any spaces.
- e.g., 111_111_111 (this is completely fine and acceptable)
- 111 1 11 (this on the other hand would throw an error)

print(1_111_111)  # use underscores to improve readability of large numbers
print(-1_111_111)

### Octal and hexadecimal numbers

- If an integer number is preceded by an 0O or 0o prefix (zero-o), it will be treated as an octal value. This means that the number must contain digits taken from the [0..7] range only.
- The print() function does the conversion automatically.


```python
print(0o123)

```

    83
    

- The second convention allows us to use hexadecimal numbers. Such numbers should be preceded by the prefix 0x or 0X (zero-x).

- 0x123 is a hexadecimal number with a (decimal) value equal to 291. The print() function can manage these values too.


```python
print(0x123)

```

    291
    

### FLOATS

- They are the numbers that have (or may have) a fractional part after the decimal point
- e.g., 2.5, 0.4, -0.5




```python
print(-0.4)  # the dot is what qualifies this to be a float
print(4)     # this is an integer
print(4.0)   # this is a float
```

    -0.4
    4
    4.0
    

### REPRESENTING STRINGS


```python
print("this is a string!")
print("this is also\na string!")

#if the string contains double quotes, then enclose the string within single quotes

print('my name is "Monty Python"!')

#or another way of doing the same with double quotes would be

print("my name is \"Monty Python\"!")
```

    this is a string!
    this is also
    a string!
    my name is "Monty Python"!
    my name is "Monty Python"!
    

### BOOLEANS


```python
#Booleans are True or False values
#True equates to a value of 1 and False to a value of 0

print(1==2)
print(1!=2)

print(True>False)
print(True<False)
print(True!=False)
print(True==False)
```

    False
    True
    True
    False
    True
    False
    

### SUMMARY

1. Literals are notations for representing some fixed values in code. Python has various types of literals - for example, a literal can be a number (numeric literals, e.g., 123), or a string (string literals, e.g., "I am a literal.").

2. The binary system is a system of numbers that employs 2 as the base. Therefore, a binary number is made up of 0s and 1s only, e.g., 1010 is 10 in decimal.

- Octal and hexadecimal numeration systems, similarly, employ 8 and 16 as their bases respectively. The hexadecimal system uses the decimal numbers and six extra letters.

3. Integers (or simply ints) are one of the numerical types supported by Python. They are numbers written without a fractional component, e.g., 256, or -1 (negative integers).

4. Floating-point numbers (or simply floats) are another one of the numerical types supported by Python. They are numbers that contain (or are able to contain) a fractional component, e.g., 1.27.

5. To encode an apostrophe or a quote inside a string, you can either use the escape character, e.g., 'I\'m happy.', or open and close the string using an opposite set of symbols to the ones you wish to encode, e.g., "I'm happy." to encode an apostrophe, and 'He said "Python", not "typhoon"' to encode a (double) quote.

6. Boolean values are the two constant objects True and False used to represent truth values (in numeric contexts 1 is True, while 0 is False.

### OPERATORS - DATA MANIPULATION TOOLS


```python
#operators help with manipulating the data by allowing the user to perform arithmetic operations 
#they can be +, -, *, /, //, %, **

print(2+2)

print(4-2)

print(4*2)

print(4/2)

print(13//10)

print(10%5)

print(2**2)
```

    4
    2
    8
    2.0
    1
    0
    4
    

### OPERATOR PRECEDENCE

1. _An expression is a combination of values (or variables, operators, calls to functions ‒ you will learn about them soon) which evaluates to a certain value, e.g., 1 + 2._


2. _Operators are special symbols or keywords which are able to operate on the values and perform (mathematical) operations, e.g., the * operator multiplies two values: x * y._


3. _Arithmetic operators in Python: + (addition), - (subtraction), * (multiplication), / (classic division ‒ always returns a float), % (modulus ‒ divides left operand by right operand and returns the remainder of the operation, e.g., 5 % 2 = 1), ** (exponentiation ‒ left operand raised to the power of right operand, e.g., 2 ** 3 = 2 * 2 * 2 = 8), // (floor/integer division ‒ returns a number resulting from division, but rounded down to the nearest whole number, e.g., 3 // 2.0 = 1.0)_


4. _A unary operator is an operator with only one operand, e.g., -1, or +3._


5. _A binary operator is an operator with two operands, e.g., 4 + 5, or 12 % 5._


6. _Some operators act before others - the hierarchy of priorities:_


_the ** operator (exponentiation) has the highest priority;
then the unary + and - (note: a unary operator to the right of the exponentiation operator binds more strongly, for example 4 ** -1 equals 0.25)
then: *, /, and %,
and finally, the lowest priority: binary + and -._

7. _Subexpressions in parentheses are always calculated first, e.g., 15 - 1 * (5 * (1 + 2)) = 0._


8. _The exponentiation operator uses right-sided binding, e.g., 2 ** 2 ** 3 = 256._


```python
#**, Unary (+,-) , * , / , //, %, Binary (+,-_)
print(9 % 6 % 2)

#There are two possible ways of evaluating this expression:

#from left to right: first 9 % 6 gives 3, and then 3 % 2 gives 1;
#from right to left: first 6 % 2 gives 0, and then 9 % 0 causes a fatal error.
#In case of two operators with equal precedence - go from left to right except for the expoentiation operator
#which uses right-sided binding

print(2 ** 2 ** 3)

print("Result of 7/3 : ",7/3)   # the result is always a float
print("Result of 7//3 : ",7//3)  # floor division, when it is a negative result, this gets ROUNDED to the LESSER INTEGER
print(-1//2)

```

    1
    256
    Result of 7/3 :  2.3333333333333335
    Result of 7//3 :  2
    -1
    

### VARIABLES

- _A variable is a named location reserved to store values in the memory. A variable is created or initialized automatically when you assign a value to it for the first time._


- _Each variable must have a unique name ‒ an identifier. A legal identifier name must be a non-empty sequence of characters, must begin with the underscore(_), or a letter, and it cannot be a Python keyword. The first character may be followed by underscores, letters, and digits. Identifiers in Python are case-sensitive._


- _Python is a dynamically-typed language, which means you don't need to declare variables in it. To assign values to variables, you can use a simple assignment operator in the form of the equal (=) sign, i.e., var = 1._


- _You can also use compound assignment operators (shortcut operators) to modify values assigned to variables, for example: var += 1, or var /= 5 * 2._


```python
john=5
mary=6
adam=2

print(john, mary, adam)

total_apples = john+mary+adam
print("total apples:", total_apples)
```

    5 6 2
    total apples: 13
    

### INTERACTION WITH THE USER

- _The print() function sends data to the console, while the input() function gets data from the console._


- _The input() function comes with an optional parameter: the prompt string. It allows you to write a message before the user input_


- _When the input() function is called, the program's flow is stopped, the prompt symbol keeps blinking (it prompts the user to take action when the console is switched to input mode) until the user has entered an input and/or pressed the Enter key._


- _The result of the input() function is a string._


```python
anything = input("Tell me anything...")
print("Hmm...", anything, "...Really?")


```

    Tell me anything...it's cold outside!
    Hmm... it's cold outside! ...Really?
    

### TYPE CONVERSION


```python
# functions available - str(), int(), float()
anything = float(input("Enter a number: "))
something = anything ** 2.0
print(anything, "to the power of 2 is", something)

```

    Enter a number: 5
    5.0 to the power of 2 is 25.0
    

### CONDITIONALS


```python
#If Conditionals

weather = input("what's the weather like? ")
if weather == "sunny":
    print("let's go for a walk")
print("time for a nap!")
```

    what's the weather like? rainy
    time for a nap!
    


```python
#if-else

age = int(input("enter your age: "))
if age >= 18:
    print("you are eligible to vote!")
    
else:
    print("you're", str(18-age), "years too young!")
```

    enter your age: 14
    you're 4 years too young!
    


```python
#nested if-else
num1= int(input("num1: "))
num2 = int(input("num2: "))
num3 = int(input("num3: "))

if num1>num2:
    if num1>num3:
        print(str(num1), "is the greatest of the three!")
        
    else:
        print(str(num3), "is the greatets of the three!")
else:
    print(str(num2), "is the greatest of the three!")


```

    num1: 5
    num2: 10
    num3: 9
    10 is the greatest of the three!
    

### LOOPS

#### FOR LOOPS


```python
for i in range(2,8,2):
    print("The value of i is currently", i)

    
print()

for i in range(5,2,-1):
    print(i)
    

```

    The value of i is currently 2
    The value of i is currently 4
    The value of i is currently 6
    
    5
    4
    3
    

### BREAK AND CONTINUE


```python
# break - example

print("The break instruction:")
for i in range(1, 6):
    if i == 3:
        break
    print("Inside the loop.", i)
print("Outside the loop.")

print()

```

    The break instruction:
    Inside the loop. 1
    Inside the loop. 2
    Outside the loop.
    

### LOGIC AND BIT OPERATIONS


```python
#and, or, not
a = True
b = False

# and is the CONJUNCTION binary operator
print("a AND b",a and b)  
# or is the DISJUNCTION binary operator
print("a OR b",a or b)   
# not is the NEGATION unary operator
print("Negation of a is ",not a)

```

    a AND b False
    a OR b True
    Negation of a is  False
    

### LISTS

- It is an ordered and mutable collection of comma-separated items between square brackets
- Lists can be indexed and updated
- Lists can be nested
- List elements and lists can be deleted
- Lists can be iterated through using the for loop
- The len() function may be used to check the list's length
- A typical function invocation looks as follows: result = function(arg), while a typical method invocation looks like this:result = data.method(arg)


```python
my_list = ['one','two','three',4,5]
```


```python
# Grab element at index 0
my_list[0]
```




    'one'




```python
# Grab index 1 and everything past it
my_list[1:]
```




    ['two', 'three', 4, 5]




```python
# Grab everything UP TO index 3
my_list[:3]
```




    ['one', 'two', 'three']



We can also use + to concatenate lists, just like we did for strings.


```python
my_list + ['new item']
```




    ['one', 'two', 'three', 4, 5, 'new item']



Note: This doesn't actually change the original list!


```python
my_list
```




    ['one', 'two', 'three', 4, 5]



You would have to reassign the list to make the change permanent.


```python
# Reassign
my_list = my_list + ['add new item permanently']
```


```python
my_list
```




    ['one', 'two', 'three', 4, 5, 'add new item permanently']



We can also use the * for a duplication method similar to strings:


```python
# Make the list double
my_list * 2
```




    ['one',
     'two',
     'three',
     4,
     5,
     'add new item permanently',
     'one',
     'two',
     'three',
     4,
     5,
     'add new item permanently']




```python
# Again, doubling is not permanent
my_list
```




    ['one', 'two', 'three', 4, 5, 'add new item permanently']




```python
#len function
len(my_list)

#removing elements from a list
#before removing
print(my_list)
my_list.append('add new item permanently')
#after removing
print(my_list)

#using del
del my_list[2]


```

    ['one', 'two', 'three', 4, 5]
    ['one', 'two', 'three', 4, 5, 'add new item permanently']
    


```python

```
