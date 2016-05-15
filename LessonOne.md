# Operating Systems

The operating system, or OS, does basic things on your computer. Other programs work on top of the OS. With the OS, you can create folders (directories) and files of various types. 

The Mac OS is similar to an OS called Unix. It is a Unix-flavored OS. There is a programming language called unix that you use to do things with the OS. It's helpful to learn a few of these unix style commands so that we can: 

- start up a python command line
- create, save, and edit text files containing programs and data
- process data from other sources so that we can run computer programs on it
- much more

To get started: 

1. Open a terminal window. In the Search form type: `terminal`. 
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







