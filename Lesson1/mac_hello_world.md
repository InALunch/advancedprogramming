# Our First Python Program and Using the Terminal

Okay! You made it this far! Now, we get to write our first program in Python. Before we do that though, we need to get a bit more acquainted with our scary but useful friend, the terminal.

<img src="hacking.gif" width=50%>

> (This actually isn't at all what working with the terminal looks like. It's just what it feels like the first few times you use it.)

## So, what is the terminal?

The first time I had to use the terminal, I thought of the movies where you see hackers frantically typing in their keyboard as green text frantically sprays up the screen over a black background and wondered if that was it was going to be like. Spoiler alert: it's not.

Here is the dictionary definition of the terminal, according to dictionary.com:

> Any device for entering information into a computer or receiving information from it.
 
That's a bit vague, but that's essentially all it is. It's a way of us interacting with the computer in a different way than clicking and scrolling through windows. In some ways, it's more limited and difficult to use, but in other ways, as you'll learn throughout this class, it makes things a lot easier and gives us much more capabilities, especially for programming.

So let's go ahead and learn some of the basics.

Type `ls` into the terminal and hit "enter".

You should see something that looks like this:

<img src="ls.png" width=50%>

*What just happened?*

`ls` stands for "list", and what you just did is list all the files of the directory you're currently in. That's another thing to remember about the terminal: you always have a directory that you're in at any given point. To figure out what directory that is, you can type the command, `pwd` into the terminal. This stands for "print work directory". After doing this, you should see similar to:

    /Users/nshak

And if you open up Finder and look in that same folder that you're in in the terminal, you should see the same folders and files as were printed out by `ls`. The terminal is actually a lot like a text version of the Finder in many ways, if that makes it easier to think about.

Just to prove it to you, here's what that folder looks like for me in Finder:

<img src="finder.png" width=50%>

Now, to learn one of the most important terminal commands we'll be using. Go type this command into the terminal:

    cd Documents

Now, type `ls` into the terminal. Notice anything different? That's because we just entered the "Documents" folder. If you want to confirm that, go ahead and try the `pwd` command to confirm that. If you didn't already guess it, `cd` stands for "change directory".

Another thing, if you ever want to go up a level in folders (out of the directory you're currently in), use this command:

    cd ..

You just learned a couple of the most important terminal commands for navigating around. Feel free to take some time using `cd` and `ls` and `pwd` to navigate all over the place while feeling like a [real hacker](http://geektyper.com/tegnio/).  

> Pro tip: if you ever want to quickly return to your "home" directory, you can just type `cd` with nothing after it, and it will take you there.

> Pro tip: if you are really deep into a directory structure, you can jump out of multiple directories in one line. `cd ../` goes up one level, `cd ../../` goes up two levels, etc.

Here's a list of the commands we've learned so far, just so you remember:

* `ls` - list files and directories
* `cd` - change directory
* `pwd` - print working directory

> Pro tip: as you're in the middle of typing file and directory names, try pressing tab. This will cause the terminal to autocomplete what you're typing if you've typed enough letters for it to narrow down what you're typing.

Once you're bored of `cd`ing and `ls`ing around, it's time for...

## Creating your First Python Program

Go ahead and navigate to your Documents folder (or whatever other folder you'd like to do this in). Now, type the following command:

    mkdir mycode

If you use `ls` again, you'll see that a folder called "mycode" now exists. That's because the `mkdir` command just created it. Go ahead and `cd` into that new folder you just created.

Now, we're going to need to install a program called Sublime Text 2 if you don't already have it on the computer. You can check if you have this installed already by typing in the terminal:

    which subl

`which` is a command that checks where certain programs are stored on your computer. If nothing shows up, it means it isn't installed yet. Follow [these instructions](installsublmac.md) to install it. If it's already installed, you should see something like:

    /usr/local/bin/subl

Next, we're going to create our Python file. Use the following command to do so:

    subl helloworld.py

This should open an empty Sublime Text 2 window. We need the `.py` to tell it that it's a python file. If you haven't used Sublime Text before, it's a text editor for your code. (Think Microsoft Word, but for code.) You'll come to appreciate it in all it's awesomeness as we go further through the class.

Alright, ready for our first Python program?

For this, all we're going to do is write one simple line of Python code in Sublime Text. Here it is:

    print("hello world!")

It should look like this:

![](helloworld.png)

After you type that, hit "command-s" to save. Make sure the circle on the tab turns to an "x" like you see in the picture. That means all your changes were saved.

*Okay, ready to run it?*

Go back to the terminal and run the following command:

    python helloworld.py

> Tip: try pressing tab after you've typed a couple characters of "helloworld.py".

This is how we run Python files. You should see the following:

<img src="helloworldoutput.png" width=70%>

Which means you ran your program, and you're seeing the output of that program. Congrats, you just wrote your first program! That's all for this lesson!

[Click here to move on to Lesson 2!](../Lesson2)