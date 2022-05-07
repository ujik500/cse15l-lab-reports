# Week 6 Lab Report
## Streamlining SSH Configuration
The basic command to connect to the ieng6 remote server (`$ ssh cs15lsp22___@ieng6.ucsd.edu`) is very long, and annoying to type out every time one wants to connect. So, to make this process easier in the future, we can add some lines of text to the .ssh/config file. To accomplish this, my partner and I opened the .ssh folder using VS Code and pasted the appropriate text into it. This is what that file looks like when we print out its contents with `cat` on the command line:

![Image1](week6pic1.PNG)

The first (non-indented) line - in this case `Host ieng6` - specifies the "alias" of the computer we are trying to connect to. This is the name we now use in the simplified command, as shown below:

![Image2](week6pic2.PNG)

In addition to `ssh`, this alias can also be used with the `scp` command to copy files from our local computer to the remote one. An example of that is shown below, copying our group's MarkdownParse.java to the ieng6 computer: 

![Image3](week6pic3.PNG)

We can check to make sure this process worked correctly by logging into the remote server again with `ssh` and using the `ls` command to verify the file we want is actually there. As shown below, it worked successfully!

![Image4](week6pic4.PNG)

## Setup GitHub Access from ieng6

## Copy Whole Directories with `scp -r`
