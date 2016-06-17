# Functions

- jupyter notebooks
- writing longer programs

## Previous lesson recap

- what is syntax
- the type function
- conditionals
- for loops

## Another type: Boolean

We have already used booleans in conditional statements. A boolean variable is one that has one of two values: True or False. 

We can set x to be a boolean. At the command line, try: 

`x = False`

`type(x)`

Try these other booleans: 

`y = (5 > 3)`

`z = 5 > 7`

Then: 

`print y, z`

The parentheses are not necessary, but make things easier to read. 

Booleans follow rules of logic and truth tables. Try out the following code: 

`dessert = 3`

`allergy = 2`

`sad = dessert < 2 or allergy == 2`

`happy = (dessert > 2) and (allergy < 2)`

`if happy:
      print "Smile"`
     
What is the result? 

Try:

`if sad:
     print "boo hoo"`
     
What is the result?

## Jupyter notebooks

The rest of the lesson is to get jupyter notebooks running and write code in a jupyter notebook. 

At the unix prompt, make yourself a new directory called notebooks: 

`mkdir notebooks`

Navigate to this directory:

`cd notebooks`

You might have jupyter already installed. Type: 

`jupyter notebook`

- if you are taken to a list in your browser, jupyter is working. 
- If there is a "command not found" message, jupyter has to be installed. 

A good way to do this is to create a virtual environment and install jupyter in there. This will shelter your computer from your python activities (and shelter your python activities from your computer). 

The `virtualenv` package might already be installed. If it is not, type: 

`easy_install virtualenv`

If it installs correctly, you can create a new virtual environment. Let's create an environment called venv: 

`virtualenv venv`

Having created `venv`, we now activate it: 

`source venv/bin/activate`

Your unix prompt should now begin with `(venv)` indicating that you are inside the virtual environment `venv`. 

Now install `jupyter`: 

`pip install jupyter`

When that is done, start up your notebook server: 

`jupyter notebook`

     




