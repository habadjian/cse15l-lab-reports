
# Week 4 Lab Report: Syptoms and Bugs

## Code Change #1:

* The first problem we encountered was an infinite loop. A link to the failing test can be found **[here](https://github.com/habadjian/markdown-parse/blob/main/test-file.md)**.
  
![CodeChange1](images2/codeChange1.png)

* The infinite loop looked like this:
  
![InfiniteLoop](images2/infLoop1.png)

* The way we fixed it was by adding an ```if``` statement that checked if ```nextOpenBracket``` was equal to -1. If it was, it would return ```toReturn```.
  
![Working Program](images2/workingProgram.png)

* The bug in our program was apparent because we didn't have the ```if``` statement that checked if the index was -1. The symprtom was the infinite loop in this case and the failure inducing output was not having a closed bracked in **test-file.md**.

***

## Code Change #2:

* Our second problem was with the tester file for the week 4 Lab. When we tried to read the file contents in the tester file, we would get this error message(Link **[here](https://github.com/habadjian/markdown-parse/blob/main/MarkdownParseTest.java)**):
  
![Image](images2/IOEXC.png)
  
![Git](images2/Git.png)

* Error Message:
  
![Error2](images2/errorMessage2.png)
  
* We were able to fix this by adding ```throws IO Exception``` after the parenthesis in the method header.

* Here is an image of the fixed file:
  
![Fixed file](images2/fixedmessage.png)

* The bug here was caused by not having the ```throws IO Exception``` in the method header. The symptom was the code not being able to compile due to the Exception not being able to be thrown. 

***

# Coding Change #3:

* The last thing we tested for was what would happen if there was other text in the test files. The test we used can be found **[here](https://github.com/habadjian/markdown-parse/blob/main/test2.md)**.

* We did this by adding the line ```System.out.println(currentIndex);```. This line helped us see how many links were being added to the arraylist and if any text was being added as well. 

![Image](images2/added.png)

  
![Image2](images2/Git3.png)

* Output of change made:
  
![SysoutForLoop](images2/outputForSysout.png)
  
* The bug we were trying to fix was adding text to the test file and seeing if the program would count that as a link. The symptoms were the text being added to the array. We were able to test for this by printing currentIndex out for each iteration through the while loop in order to see how many times a link was added to the array. 

![Image3](images2/Image3.png)

