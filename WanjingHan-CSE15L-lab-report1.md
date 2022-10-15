1. Installing VScode
 
 ![Image](https://github.com/wahanucsd/cse15l-lab-reports/blob/main/Screen%20Shot%202022-10-14%20at%206.47.13%20PM.png)



I installed VScode before the lab. I downloaded the VScode installer from this link: https://code.visualstudio.com/. Then I clicked download and choosed “Mac- Apple Silicon”.
After finishing the installation, I clicked VScode in my laptop launchpad.



 
2. Remotely Connecting


![Image](https://github.com/wahanucsd/cse15l-lab-reports/blob/main/Screen%20Shot%202022-09-30%20at%2011.48.43%20AM.png)



I used this link to find my username and password:https://sdacs.ucsd.edu/~icc/index.php.
Then I typed my UCSD username and PID and clicked submit.
Then I clicked my CSE15L username, the form is cs15lfa22zz. My username is cs15lfa22dm.
Then I clicked “change your password”.
For the question “Change My Tritonlink Password”, I choosed “no”.
For the question “Change Course-Specific Passwords”, I choosed “yes”.
Then I entered my current password and new password I want to set and clicked enter after typing the new password.
Then I wait about 15 to 30 minutes for changing password.

I used VSCode to open the terminal. After opening the VSCode, there is an option called “terminal” on the top of screen. I clicked “new terminal” to open a new terminal.

Then I typed a command called “ssh cs15lfa22dm@ieng6.ucsd.edu” into terminal.
Then I saw this in the terminal : “The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?”
Then I typed “yes”.
Then I entered my password and connected to the remote server.






I changed the password for three times. I spend almost 24 hours to login. All of us saw “You are using 0% CPU on this system.”. However, all of us have different number in “Time”, “Users”, “Load”, and “Average”.




3. Trying Some Commands

![Image](https://github.com/wahanucsd/cse15l-lab-reports/blob/main/Screen%20Shot%202022-09-30%20at%2012.22.58%20PM.png)


The “cd <path>ls” command could change the working directory. The “<path>” is the place where the file and folder in filesystem. 
The “ls <path>” command could list all the files and folders. When the directory is my own computer, this command will list all the files of my laptop. When the directory is remote, this command will list all the files of the remote directory.
I used these commands: cd ~, cd, ls -lat, ls -a, ls <directory> according to the instructions.



4. Moving Files with scp

![Image](https://github.com/wahanucsd/cse15l-lab-reports/blob/main/Screen%20Shot%202022-09-30%20at%205.12.18%20PM.png)
![Image](https://github.com/wahanucsd/cse15l-lab-reports/blob/main/Screen%20Shot%202022-09-30%20at%208.29.47%20PM.png)

First I created a file called “WhereAmI.java”.
Then I copied some code from the instruction of lab 1. The code is: “
class WhereAmI {
  public static void main(String[] args) {
    System.out.println(System.getProperty("os.name"));
    System.out.println(System.getProperty("user.name"));
    System.out.println(System.getProperty("user.home"));
    System.out.println(System.getProperty("user.dir"));
  }
}”. 
Then, I entered “scp WhereAmI.java cs15lfa22dm@ieng6.ucsd.edu:~/”using my own computer directory in the terminal. Then I used these commands: “javac WhereAmI.java” and “java WhereAmI” using my own computer directory in the terminal. 

Then I had to ssh to use these commands on the remote server.
First I used the command “ls” to check whether the “WhereAmI.java” file is in the remote server or not. 
The I used these commands: “javac WhereAmI.java” and “java WhereAmI” on the remote server.

I spend one minute and thirty-one seconds doing these things. I think that copying and running the file for 100 times need about several minutes, maybe 15 minutes.

 


 
5. Setting an SSH Key

![Image](https://github.com/wahanucsd/cse15l-lab-reports/blob/main/Screen%20Shot%202022-09-30%20at%205.42.15%20PM.png)

First, I used the command “ssh-keygen” using my own computer directory in the terminal. 
Then I entered “/Users/wanjinghan/.ssh/id_rsa” for saving the key. 
After this, I pressed “return” for several times. 
Because I need to exit the remote server before using “scp” command. 
So I exited the server and used “ssh cs15lfa22zz@ieng6.ucsd.edu”, “mkdir .ssh”, 
and “scp Users/wanjinghan/.ssh/id_rsa.pub cs15lfa22dm@ieng6.ucsd.edu:~/.ssh/authorized_keys” to check whether I need password to login. 
After checking, I found that I don't need to use password to login. 
I found that I only use fifty one seconds to do the experiment. I saved about forty seconds.



6. Optimizing Remote Running

![Image](https://github.com/wahanucsd/cse15l-lab-reports/blob/main/Screen%20Shot%202022-09-30%20at%205.51.21%20PM.png)

First, I changed the code in the file. 
After that, I used three commands: “cp WhereAmI.java OtherMain.java”, “javac OtherMain.java” and “java WhereAmI”. 
However, I found that I could use one command to run all of these commands: “cp WhereAmI.java OtherMain.java; javac OtherMain.java; java WhereAmI”. 
This could save time for use. After this, my friend told me that we could use up arrow counts to use the last command in the terminal. 
I think these could save a lot of time and work for use.

