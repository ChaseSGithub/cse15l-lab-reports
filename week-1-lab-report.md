**Hail, traveler.**  
I see you are looking for information regarding remote connections in **CSE 15L**  
Allow me to be of assistance.  
  
  **Step 1**
First and foremost, lets make sure you're situated with **Visual Studio Code,** or **VS Code** for short.  
Follow this link here [VS Code Download](https://code.visualstudio.com/) to download and get things setup on your computer.  
Once opening it and following the given prompts, you should come across a screen that looks like this:  
![VS Code](VSCodeImage.png)  
  
**Step 2**  
Once you've got VS Code situated, lets use it to connect to the 15l servers remotely.  
In VS Code, navigate towards the top bar with drop down menus until you find yourself at the one called **termnial**  
Click on it and then click on the option **New termianl*  
Once doing this, the terminal should appear on the bottom half of the screen.  
To login to the remote server, type the following command into the terminal  
  
  **ssh cse15lfa22zz@ieng6.ucsd.edu**  
    
replacing the **"zz"** with the two letters in your given username.  
After doing so, you should be prompted with terminal messages that look similar to this:  
![Terminal Post Login](TerminalLogin.png)  
  
This will be the indication that you have successfully logged in to the remote server.  
  
**Step 3**  
Now, we are going to attempt to try a few commands. There is a list of commands that you can try including:  
-cd ~  
-cd  
-ls -lat  
-ls -a  
-ls <directory> (with the directory being **/home/linux/ieng6/cs15lfa22/cs15lfa22abc** where "abc" is one of the other group member's username  
-cp /home/linux/ieng6/cs15lfa22/public/hello.txt ~/  
-cat /home/linux/ieng6/cs15lfa22/public/hello.txt  
    
 The command that I chose to use is **ls -lat** which producing a result like this, listing files in the directory laterally  
  ![First Command](firstCommand.png)  
    
  **Step 4**  
  Unfortunately, here is where I happened to run into some problems.  
  I had quite a bit of trouble when it came to logging in to the remote server but I was able to get it to work **a single time**  
  Following the instructions post **Step 3** however, prompts you to logout so that you may run commands from the client.  
  I was unable to login another time and have still been unable to do so even from my home computer, so I will try my best to describe the process without screenshots!  
    
  For this next step, you will be using the **scp** command in order to copy files from the client to the server.  
  The first step in this process is creating a file on **VS Code** named **WhereAmI.java**  
  In the file we will be creating a class called **WhereAmI"" and input the following information in it to properly print the information we need.  
  It should look something like this:  
    
  class WhereAmI {  
    public static void main(String[] args) {  
      System.out.println(System.getProperty("os.name"));  
      System.out.println(System.getProperty("user.name"));  
      System.out.println(System.getProperty("user.home"));  
      System.out.println(System.getProperty("user.dir"));  
    }  
  }  
    
  Once doing this and **saving the file**, you should be able to input the following command into the terminal:  
  scp WhereAmI.java cs15lfa22zz@ieng6.ucsd.edu:~/  
  Once again, replacing the "zz" with the two letters in your actual username  
    
  Once logging back onto the remote server, you should find this file by using **ls** to list the files in the home directory!  
    
  **Step 5**  
  For step 5, we are going to set up an **SSH Key** in order to bypass that repetitive task of failing to input your password!  
  The first step in this process is to run the following command on your client, that being:  
  $ **ssh-keygen**  
  Once running this command, you will be show information regarding the key that is being generated. This process then creates two files on your system, **id_rsa** and **id_rsa.pub**, being the private key and public key respectively.  
    
  Next, on your client, login just as you have before using the ssh command followed my your username@ieng6.ucsd.edu and then type in your password as you are prompted  
  Once on the server, enter the following commands:  
  **mkdir .ssh**  
  **<logout>**  
  Which should then return you to the client, where finally you can run  
  **scp /Users/joe/.ssh/id_rsa.pub cs15lfa22@ieng6.ucsd.edu:~/.ssh/authorized_keys**  
  Once again, using your username and the above path  
    
  *Step 6**
  For this last step, there are just a few tips and tricks when it comes to running commands on a remote server  
  For one, you can follow your ssh login command with a command in parentheses in order to run that command upon login  
  For example:  
  **ssh cs15lfa22@ieng6.ucsd.edu ""ls -lat""**  
  will run the ""ls -lat"" command upon login, producing the results shown in the screenshot from **Step 3**  
  Another tip is the fact that you can input semicolons between commands in order to run multiple commands consectuively!  
  Such as in:  
  **cp WhereAmI.java OtherMain.java; javac OtherMain.java; java WhereAmI**  
    
  With this, you'll be on your way to becoming a remote server **Superstar!**
  
  
