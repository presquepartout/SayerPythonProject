# Control Structures

- conditionals
- loops

## Previous lesson recap

- little bit of `unix`
- little bit of the Python command line
- different types of data: `int`, `float`, `str`, `list` - are there more types? Yes
- variables - easy to assign
- arithmetic - different for `int` and `float`
- the print statement
- running first program

## What is syntax? 

A computer program is a list of statements. Each statement is like a sentence that tells the computer to do something. 
We have already seen statements in Python: 

`>>>7 + 2`

means add 7 and 2, and print the result 9. 

Syntax is the set of rules that your statements must follow in order for Python to interpret them correctly. 

If you are on the Python command line and type: 

`7 plus 2` 

and press Enter, what happens? 

Try: 

`seven + 2`

What happens? 

Try: 

`"seven" + 2`

What happens?

An example of syntax you've already encountered is the list syntax. A list in Python is enclosed in square brackets [ and ]. 
The members of a list are separated by commas. The list [1, 2, 3] has three items; the list ["123"] has one item. 

Can you list any other examples of syntax in Python that you have already encountered? 

## The `if` statement

Suppose you want to add 10 to x if x < 5, otherwise, subtract 7 from x. Here is the syntax: 

```
if x < 5: 
    x = x + 10
else: 
    x = x - 7
```

The colon : and the indentation are important. Indent four spaces. 
At the python prompt, type out the code as follows: 

```
x = 2
if x < 5: 
    x = x + 10
else: 
    x = x - 7
    
print x
```

See if it does what you expect. 

There is special syntax for the "=" case. Suppose you want to multiply x by 10 if x = 2. 

```
if x == 2: 
    x = x*10
print x
```
Try some examples and see if they do what you expect. 

## The `for` loop

The `for` loop is a program that runs through an iterable object, and does something for each value in the iterable object. 

We will defer the definition of "iterable object" for now and look at some examples: 

#### List example of `for` loop: two flavors

Write and execute this code at the python prompt: 

```
x = [2, 3, 4]
for e in x:
   print x*5
```

See what happens. Another example: 

```
stringy = "aaapple"
for char in stringy: 
    print char
```

A digression about lists: lists and other iterable objects have indexes by which you can reference items within the list. 

What does this mean? Using the example list x above, try the following code: 

```
x[0]
```

Alternatively 

```
print x[0]
```

Try also x[1], x[2], and x[3]. See what happens. 

Try: 

```
for i in [0, 1, 2]:
    print x[i]*5
```

The above should be exactly the same as some code you tried earlier. 

The value within the square brackets is called an **index**. 

Now that you've seen some examples, here is a short recap: 
- the syntax of a `for` loop is: 

```
for item in <iterable>:
    code indented 4 spaces
    more code if needed
```

The nice thing about the `for` loop is that it comes to a stop by itself, when done with all of the items in the iterable. 

### Exercises - do these in the python command line

1. Create a variable named zz and set it to an integer value. Write some code that will print zz if zz is negative. Test it out. 
2. Write some code that will print zz if zz is negative, and print "Hello World" if zz is positive. 
3. Write code that will print the first 8 multiples of 7. 
4. Write code that will print zz if it is a multiple of 2. Otherwise it will print "Error. This number is odd." Hint: remember the difference between zz/2 and zz/2.0
5. Write code that counts the number of letters in a word. 

