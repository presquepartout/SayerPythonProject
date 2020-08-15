# Lesson One

- Basics about operating systems
- Writing your first python program

## Operating Systems

The operating system, or OS, does basic things on your computer. Other programs work on top of the OS. With the OS, you can create folders (directories) and files of various types. 

The Mac OS is similar to an OS called Unix. It is a Unix-flavored OS. There is a programming language called unix that you use to do things with the OS. It's helpful to learn a few of these unix style commands so that we can: 

- start up a python command line
- create, save, and edit text files containing programs and data
- process data from other sources so that we can run computer programs on it
- much more

To get started: 

1. Open a terminal window. In the Spotlight Search form type: `terminal`. 
2. You'll get a new window with a command line. Type: `pwd` 

The `pwd` command tells you where you are. It stands for `print working directory`. If you are using your own machine and you have your own user account named MeMyself, the output of your command should be something like this: 

`/Users/MeMyself`

This particular directory has a special name: your home directory. 

Here are some simple commands to try out: 

### Folders
Make a new folder called `mycode`: 

`mkdir mycode`

To remove a folder: 

`rmdir mycode`

### Navigate to and from folders

Create a few folders in your home directory. 

To go inside the folder `mycode`:

`cd mycode`

If this command fails, you are probably in a different place from your home directory. Use the command `pwd` to find out where you are. 

To go up a level (back out to your home directory):

`cd ..`

Your home directory has a special name: `~`

To go home from any directory: 

`cd ~`

You can find out where you are at any point by typing: `pwd`

Putting it all together: You can go to your `mycode` directory this way: 

`cd ~/mycode`

### Creating text files

Navigate to your mycode folder: 

`cd mycode`

We will use a text editor called `vim` to make files. 

Type: `vim newfile.txt`

The above command starts up the vim editor. To insert text into the file, type `i`

After typing `i` type: 

`Hello World`

`This is my first text file.`

Then press the `Esc` key and type: 

`:wq`

This will save your file and exit. 

### Listing contents of a folder

To see what is inside a folder, type: `ls`
(letter lowercase L and lowercase s)

If you do this inside your `mycode` folder, what do you see? 

If you navigate to your home folder and type `ls`, what do you see? 

Here is some output from my computer: 

`atom:mycode memyself$ pwd`

`/Users/memyself/mycode`

Above is the result of the `pwd` command. 

Below is the result of the `ls` command: 

`atom:mycode memyself$ ls`

`newfile.txt`

## The Python Command Line

Navigate to your `mycode` folder and type: `python`

This will put you in python command-line mode. You will see a prompt: `>>>`
At this prompt, you can type commands to your python interpreter and it will execute them. 

### Simple math

Python can do arithmetic. Try: 

`>>> 7 + 2`

Python can add two integers for you. Python can also multiply. Type the following and press return. 

`8*3`

Python can evaluate algebraic expressions:

`(1 + 4 + 5) / 2`

Python can print. Try: 

`print 15*3`
Above is for Python 2. If you're using Python 3: 
`print(15*3)`

Also try: 

`print "15*3"`

If python 3: 
`print("15*3")`

What is the difference between the two `print` statements? 

Notice some things about the way Python does arithmetic:

Try: 
`8 / 2`

Compare it with: 
`9 / 2`

Do you get the answers you expect? 

Try: 

`9.0 / 2.0`

What happened this time? (In Python 2, you should get a different answer from `9 / 2`, in python 3 they are the same). 

In Python, 9 and 9.0 are two different `types` of numbers. 

`9` is an `int`. (Short for integer.)

`9.0` is a `float`. (Short for floating point number.). This name has a history in computer science that you can look up. 

`"nine"` is a `str`. (Short for string, or "string of characters".) 

### Variables

It is very easy to set a variable in Python. Type: 

`x = 4`

Now, Python believes that x stands for the number 4. As written, 4 is an int not a float. 

Now you can try: 

`x + 12` 

What is the result after you press `enter`? 

What if x is 4.0 instead? Try it. Try adding x to 12 and see what you get. 

Names of variables can be almost anything. They must begin with a letter. 

OK: `alphabet = 26`

NOT OK: `26a = 1.3`

Try out what is OK and what is NOT OK. 
You can set a variable to be a string: 

`alphabet_first4 = 'abcd'`

`print alphabet_first4`

In Python 3: 
`print(alphabet_first4)`

### Your first python program: 

Exit the python interpreter by pressing Ctrl-d. (That means simultaneously press the Control key and the `d` key.)

Create a file with vim. Type: `vim hello.py`

Get into Insert mode (by typing `i`). 

Type: 

`print "Hello World!" `

if Python 3: 
`print("Hello World!")`

Save your file and exit vim by typing: `Esc`

Followed by: `:wq`

Type `ls` in your directory and see what you have. 

Type `python hello.py` and see what happens. 




