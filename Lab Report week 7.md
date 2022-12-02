Part 1

Changing the name of the start parameter and its uses to base.
  
sequence of keys:
vim DocSearchServer.java<ENTER>
/start<ENTER>
dwibase<ESC>n<ENTER>dwibase<ESC>n<ENTER>dwibase<ESC>:wq<ENTER>

  
  
vim DocSearchServer.java [ENTER]
  
![Image](https://github.com/wahanucsd/list-examples-grader/blob/main/Screen%20Shot%202022-11-13%20at%201.54.38%20PM.png)
  
I typed this command in the terminal and then I entered the vim from this command.
  
  
  
/start <ENTER>
  
![Image](https://github.com/wahanucsd/list-examples-grader/blob/main/Screen%20Shot%202022-11-13%20at%202.09.46%20PM.png)
  
I typed this command for searching "start" in vim.
  
  
  
  
dw
  
![Image](https://github.com/wahanucsd/list-examples-grader/blob/main/Screen%20Shot%202022-11-13%20at%202.11.49%20PM.png)
  
I typed this command for deleting the first "start".
  
  
  
ibase
  
![Image](https://github.com/wahanucsd/list-examples-grader/blob/main/Screen%20Shot%202022-11-13%20at%202.13.30%20PM.png)
  
I typed this command to enter insert mode and add "base".
  
  
  
  
<ESC>
  
![Image](https://github.com/wahanucsd/list-examples-grader/blob/main/Screen%20Shot%202022-11-13%20at%202.14.12%20PM.png)
  
I typed this to exit insert mode.
  
  
  
  
n <ENTER>

![Image](Screen%20Shot%202022-11-13%20at%202.18.00%20PM.png)
  
I typed this to find the next "start".

  
  
  
dw
  
![Image](https://github.com/wahanucsd/list-examples-grader/blob/main/Screen%20Shot%202022-11-13%20at%202.18.49%20PM.png)
  
I typed this command for deleting the next "start".
 
  
  
ibase
  
![Image](https://github.com/wahanucsd/list-examples-grader/blob/main/Screen%20Shot%202022-11-13%20at%202.20.49%20PM.png)
  
I typed this command to enter insert mode and add "base".
 
  
  
  
  
<ESC>
  
![Image](https://github.com/wahanucsd/list-examples-grader/blob/main/Screen%20Shot%202022-11-13%20at%202.22.08%20PM.png)
  
I typed this to exit insert mode.  
  
  
  
  
n <ENTER>
  
![Image](https://github.com/wahanucsd/list-examples-grader/blob/main/Screen%20Shot%202022-11-13%20at%202.23.29%20PM.png)
  
I typed this to find the next "start".  
  
  
  
  
dw
  
![Image](https://github.com/wahanucsd/list-examples-grader/blob/main/Screen%20Shot%202022-11-13%20at%202.24.03%20PM.png)
  
I typed this command for deleting the next "start".  
  
  
  
  
ibase
  
![Image](https://github.com/wahanucsd/list-examples-grader/blob/main/Screen%20Shot%202022-11-13%20at%202.24.36%20PM.png)
  
I typed this command to enter insert mode and add "base".
  
  
  
  
<ESC>
  
![Image](https://github.com/wahanucsd/list-examples-grader/blob/main/Screen%20Shot%202022-11-13%20at%202.25.14%20PM.png)
  
I typed this to exit insert mode.  
  
  
  
  
:wq <ENTER>
  
![Image](https://github.com/wahanucsd/list-examples-grader/blob/main/Screen%20Shot%202022-11-13%20at%202.26.02%20PM.png)
  
![Image](https://github.com/wahanucsd/list-examples-grader/blob/main/Screen%20Shot%202022-11-13%20at%202.26.34%20PM.png)
  
  
I exit the vim and return to my terminal. 
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
Part 2

goal: In DocSearchServer.java, in method getFile, I want to change the "It's a folder" to "It's not a folder".
  
strategy 1
I only used 12 second. Because I found "It's a folder" easily and I just added a "not". Then I copied the code of scp.
  
  
strategy 2
I spend 28 second. Although I already logged into my ssh sesion, I still spend about 20 in vim. Since I entered in normal mode and insert mode to change the code. Moreover, I need to exit to my terminal and run bash.
  
  
Which of these two styles would you prefer using if you had to work on a program that you were running remotely, and why?
I perfer strategy 1 one because vim is a little bit hard for me. 
  
What about the project or task might factor into your decision one way or another? (If nothing would affect your decision, say so and why!)
If I need to change many parts of the code or I have many files to change, I will choose the strategy 2 because vim could help me to find some specific code really fast.
