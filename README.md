# Instruction Project

## Description
The purpose of these instructions is to teach you how to navigate the terminal and create a simple Python program. This is a basic introduction to the terminal and Python programming.

## Materials
To complete this tutorial successfully, you will need to have the following:  
- A computer with a UNIX-terminal open. Any Mac or Linux terminal will work.
> If you are using Windows, you must use the Windows Subsystem for Linux (WSL) or terminal emulator such as Git Bash.
- Your machine must have python installed

## Steps
    
Learn to navigate the terminal.
Main commands:  
`cd` - change directory  
`ls` - list files  
`mkdir` - create directory  
`touch` - create file  
`nano` - edit file

1. Start with open terminal

2. The `cd` command stands for *change directory*. It is used to navigate through directories.  
To go to the home directory, type `cd` and press enter.

3. We should now be in the home directory. This is sometimes called the *root*. It would be nice to see what files and folders are in the root.  
Run `ls` to list all files in that directory.

4. We're going to navigate into one of these folders to practice changing directories.  
Pick a folder and run `cd folder_name` to go into that folder. *Replace `folder_name` with the name of the folder you want to go into*.

5. Run `ls` to see the files and folders in the directory you just navigated to.

6. To move backwards a directory, you can run `cd ..`. This will take you back to the previous directory.  
Run `cd ..` to go back one directory.

You can now navigate through directories in the terminal. Now it's time to create our own folder.

7. Let's create a folder in this directory. The `mkdir` command stands for *make directory*. We're going to create a folder called `instruction_project`. 
Run `mkdir instruction_project`.

8. Run `ls` to see the folder you just created. You should see `instruction_project` listed.

9. Navigate into the `instruction_project` folder by running `cd instruction_project`.

10. Run `ls` to see the files and folders in the `instruction_project` directory. It should be empty. Let's add some files.

The `touch` command is used to create files. We're going to create a file called `test.py`.

11. Run `touch test.py` to create the file.

12. Run `ls` to verify that the file was created.

We can edit this file in the terminal by using a command called `nano`. We're going to open the `test.py` file and write a simple Python program.

13. Run `nano test.py` to open the file in the terminal.

This may look confusing at first, but it's actually quite simple. We are going to write a few python commands, save the file, and then run the file. First we want to write a simple program that creates a simple integer guessing game.

14. Write the following code in the `test.py` file:
```python
import random
n = random.randrange(1,10)
while True:
    guess = int(input("Enter a guess: "))
    if guess < n:
        print("Too low, try again.")
    elif guess > n:
        print("Too high, try again.")
    else:
      break
print("Correct!")
```

15. To save the file, press `ctrl + x`. You will be prompted to save the file. Press `y` to save the file. Then press `enter` to confirm the file name.

16. Run `python test.py` to run the file. You should see "Enter a guess" printed in the terminal.

17. Run the program until you guess the number correctly and the program exits automatically. 

18. Complete the survey at https://qualtricsxm8byd6wvxh.qualtrics.com/jfe/form/SV_2huvS2HPXeqO6zQ
    
## Troubleshooting

* If a command doesn't work, or comes back with an error, make sure you typed the command correctly.
* You may get an error message telling you that you were unable to execute the python file. If this error comes up, enter python -version in the terminal. If you get a message saying that you don't have python installed, [install python](https://wiki.python.org/moin/BeginnersGuide/Download).

