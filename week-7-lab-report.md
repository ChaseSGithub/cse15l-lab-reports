The shortest set of commands needed to replace all the variations of "start" with the word "base" is:  
![pic7](cs15lab7pic7.png)

The base segment of code starts off looking like this:  
![pic1](cs15lab7pic1.png)  
  
 After pressing colon, typing %s/ and then typing start in a manner that results in this:  
 ![pic5](cs15lab7pic5.png)  
   
 You'll end up with a highlight appearing around all of the instances of that word "start" in the file:  
 ![pic2](cs15lab7pic2.png)  
   
 Then, afteter typing /base after "start", as you type it each letter, it will delete all iterations of "start"  
 and begin to type out the word you are currently typing, in this case "base"  
   
 ![pic6](cs15lab7pic6.png)  
 ![pic3](cs15lab7pic3.png)  
   
 Finally, finish out the command with /g and press <enter>, committing all of the changes:  
 ![pic7](cs15lab7pic7.png)  
  ![pic4](cs15lab7pic4.png)  
  
    
    
**Part 2**  
For the second part of this lab, the following indiciates the amount of seconds it took me to run each set of commands:  
**48 seconds** to run **scp**  
**18 seconds** to run vim after already using **ssh**  
  
This probably just stems from my difficulty with using scp and typing it out, but I prefer to already be ssh'd in regardless.  
It is easier in my brain to be in the remote place first than to try logging in remotely.  
If I wanted to make a phone call from Spain, I'd rarther go to Spain and make the call (If I could travel instantaneously) than to try and remotely call from Spain, from home  
  
  I'm not sure if there would be any implications of the task that would affect this decision, simply because it is to my understanding that  
  **scp** and **ssh** are extensions of each other, both helping you work with remote servers. If thats the case, one should be usable over the other  
  and I just prefer to ssh.
 
