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
Try out the above code as follows: 

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
```
Try some examples and see if they do what you expect. 
