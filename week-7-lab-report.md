The shortest set of commands needed to replace all the variations of "start" with the word "base" is:  
:%s/start/base/g

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
   
 Finally, finish out the command with /g and press enter, committing all of the changes:  
 ![pic4](cs15lab7pic4.png)  
  ![pic7](cs15lab7pic7.png)  

 
