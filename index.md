---
title: Shell Scripting
---


# Shell Scripting


## What is a Shell?
An Operating is made of many components, but its two prime components are: 
 1. Kernel
 2. Shell

![OS Components](https://github.com/sem1colon/Images/blob/master/ShellScripting.png)

A Kernel is at the nucleus of a computer. It makes the communication between the hardware and software possible. While the Kernel is the innermost part of an operating system, a shell is the outermost one. 
A shell in a Linux operating system takes input from you in the form of commands, processes it, and then gives an output. It is the interface through which a user works on the programs, commands, and scripts. A shell is accessed by a terminal which runs it. 
When you run the terminal, the Shell issues a command prompt (usually $), where you can type your input, which is then executed when you hit the Enter key. The output or the result is thereafter displayed on the terminal. 
The Shell wraps around the delicate interior of an Operating system protecting it from accidental damage. Hence the name Shell. 

## Types of Shell
There are two main shells in Linux: 
1. The <b>Bourne Shell</b>: The prompt for this shell is $ and its derivatives are listed below: 
POSIX shell also is known as sh
Korn Shell also knew as sh
<b>B</b>ourne <b>A</b>gain <b>SH</b>ell also knew as bash (most popular)
2. The <b>C shell</b>: The prompt for this shell is %, and its subcategories are: 
C shell also is known as csh
Tops C shell also is known as tcsh

We will discuss bash shell based shell scripting here. 

## What is Shell Scripting?

Shell scripting is writing a series of command for the shell to execute. It can combine lengthy and repetitive sequences of commands into a single and simple script, which can be stored and executed anytime. This reduces the effort required by the end user.

Let us understand the steps in creating a Shell Script 
	1. <b>Create</b> a file using a <b>vi</b> editor(or any other editor).  Name  script file with extension <b>.sh</b>
	2. <b>Start</b> the script with <b>#! /bin/sh</b>
	3. Write some code.
	4. Save the script file as filename.sh
	For executing the script type bash filename.sh
	"#!" is an operator called shebang which directs the script to the interpreter location. So, if we use"#! /bin/sh" the script gets directed to the bourne-shell. 
Let's create a small script - 
```
#!/bin/sh
ls
```
Let's see the steps to create it - 

![Steps](https://github.com/sem1colon/Images/blob/master/vi_scriptsample(2).png)

Command 'ls' is executed when we execute the scrip sample.sh file.

## Adding shell comments
Commenting is important in any program. In Shell programming, the syntax to add a comment is
```
#comment
```
Let understand this with an example.

![comment](https://github.com/sem1colon/Images/blob/master/adding_comment.png)

#What are Shell Variables?
As discussed earlier, Variables store data in the form of characters and numbers.
Similarly, Shell variables are used to store information and they can by the shell only.
For example, the following creates a shell variable and then prints it:
```
#!/bin/sh
echo "what is your name?"
read name
echo "How do you do, $name?"
read remark
echo "I am $remark too!"
```
Let's understand,  the steps to create and execute the script:

![program](https://github.com/sem1colon/Images/blob/master/program.jpg)

As you see, the program picked the value of the variable 'name' as Joy and 'remark' as excellent.
This is a simple script. You can develop advanced scripts which contain conditional statements, loops, and functions.
Shell scripting will make your life easy and Linux administration a breeze. 
