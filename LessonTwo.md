# Control Structures

- conditionals
- loops

## Previous lesson recap

- little bit of `unix`: commands `pwd`, `cd`, `ls`, `python`
- little bit of the Python command line `>>>`
- different types of data: `int`, `float`, `str` - are there more types? Yes
- variables - easy to assign
- arithmetic - different for `int` and `float`
- the print statement
- running first program, `hello.py`

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

`7 plus 2`, `seven + 2`, `"seven" + 2` are all examples of things that a human can read but Python has trouble reading. 
Python needs statements to follow rules, and the rules must be followed without exception. We will learn the rules as we go. 
The rules of correct statements are called syntax. 

We've already encountered data types. Three examples of data types are int, float, and str. (Integer, floating point number, and string). 
You know you can add an int to an int using the plus sign. 
Can you add an int to a float? Try it. 

Can you add a string to a string? Here is how to try it: 
`>>> x = 'dog' `

`>>> y = 'cat' `

`>>> x + y `

After pressing enter, you should see: `dogcat`. 

But if you try: 

`>>> x + 2`

That would fail. You cannot add an int and a str. 

Another important data type in Python is the list. A list is an example of an array. A Python list is enclosed in square brackets [ and ]. 
The members of a list are separated by commas. The list `[1, 2, 3]` has three items - the three ints 1, 2, and 3. 
The list `["123"]` has one item - the string `"123"`. 

Can you list any other examples of syntax in Python that you have already encountered? 

## The `type` function

The reserved word `type` is a function that tells you what type of data something is. 

Try entering these statements at the python command line:  

`type(4)`

(Above means: what is the type of 4?)

`type(4.1)`

`type("4")`

`type(four)`

`type("four")`

In the case of `type(four)` Python is confused. It tried to look up four but could not find it. Python would know that "four" is a string, but it does not know what four is unless you define it. 

Try this sequence of commands: 

`four = 4.0`

`type(four)`

Now, Python knows what four is, because you have defined it. 


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
   print e*5
```

See what happens. Another example: 

```
stringy = "aaapple"
for char in stringy: 
    print char
```
#### Iterables

Both strings and lists are examples of iterable objects, or iterables. An iterable is a set of items "whose items you can name in order, from first to last". 

The "place" of an item is called its **index**. 

In the list `[4, 6, 8]`, the first item is 4. Its index is 0. If: 

` x = [4, 6, 8]`

Then: `x[0] = 4` - you can test this in Python by entering: 

The index of 6 is 1, and the index of 8 is 2. 

If: 

` s = "aaapple" `

What is `s[0]` ? 
What is `s[5]`? 

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
4. Write code that will print zz if zz is a multiple of 2. Otherwise it will print "Error. This number is odd." Hint: remember the difference between zz/2 and zz/2.0
5. Write code that counts the number of letters in a word. 

