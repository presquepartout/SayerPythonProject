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
Make a new folder called `python`: 

`mkdir python`

To remove a folder: 

`rmdir python`

### Navigate to and from folders

Create a few folders in your home directory. 

To go inside the folder `python`:

`cd python`

To go up a level (back out to your home directory):

`cd ..`

Your home directory has a special name: `~`

To go home from any directory: 

`cd ~`

You can find out where you are at any point by typing: `pwd`

### Creating text files

Navigate to your python folder: 

`cd python`

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

If you do this inside your `python` folder, what do you see? 

If you navigate to your home folder and type `ls`, what do you see? 

## The Python Command Line

Navigate to your python folder and type: `python`

This will put you in python command-line mode. You will see a prompt: `>>>`
At this prompt, you can type commands to your python interpreter and it will execute them. 

### Simple math

Python can do arithmetic. Try: 

`7 + 2`

Python can add two integers for you. Python can also multiply. Type the following and press return. 

`8*3`

Python can evaluate algebraic expressions:

`(1 + 4 + 5) / 2`

Python can print. Try: 

`print 15*3`

Also try: 

`print "15*3"`

What is the difference between the two `print` statements? 

Notice some things about the way Python does arithmetic:

Try: 
`8 / 2`

Compare it with: 
`9 / 2`

Do you get the answers you expect? 

Try: 

`9.0 / 2.0`

What happened this time? (You should get a different answer from `9 / 2`). 

That is because to Python, 9 and 9.0 are two different `types` of numbers. 

`9` is an `int`. (Short for integer.)
`9.0` is a `float`. (Short for floating point number.). This name has a history in computer science that you can look up. 
`"nine"` is a `str`. (Short for string, or "string of characters".) 

### Variables

It is very easy to set a variable in Python. Type: 

`x = 4`

Now you can try: 

`x + 12` 

What is the result? 

What if x is 4.0 instead? Try it. Try adding x to 12 and see what you get. 

Names of variables can be almost anything. They must begin with a letter. 

OK: `alphabet = 26`

NOT OK: `26a = 1.3`


### Your first python program: 

Exit the python interpreter by pressing Ctrl-d. (That means simultaneously press the Control key and the `d` key.)

Create a file with vim. Type: `vim hello.py`

Get into Insert mode (by typing `i`). 

Type: 

`print "Hello World!" `

Save your file and exit vim by typing: `Esc`

Followed by: `:wq`

Type `ls` in your directory and see what you have. 

Type `python hello.py` and see what happens. 




