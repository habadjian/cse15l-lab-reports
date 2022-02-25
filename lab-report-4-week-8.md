# Week 8 Lab Report: Debuggers

**Repositories used for this lab**

* [Link to my Repo](https://github.com/habadjian/markdown-parse)
  
* [Link to the reviewed Repo](https://github.com/mramada22/markdown-parse)

***

## Snippet 1:

* What should be produced:

![snippet1actual](images4/snippet1actual.png)
  
* Test used for both my repo and reviewed repo: 
  
![snippet1test](images4/snippet1test.png)

* My snippet 1 test output(failed):
  
![mysnippet 1 test output](images4/mysnip1testr.png)

* Reviewed repo Snippet 1 test output(failed):
  
![their snippet 1 test output](images4/theirsnip1testr.png)

* Code change answer: I believe there is a small code change that could be implemented in order to read ``` `[a.com`](url.com) ``` as a link. There could be an ```if``` statement implemented that would check for a the "``` ` ```" character before the ```nextOpenBracket``` variable. If there was a chracter, then disregard it and move on with the loop.
***
  
## Snippet 2:

* What should be produced:

![snippet2actual](images4/snippet2actual.png)
  
* Test used for both my repo and reviewed repo: 
  
![snippet2test](images4/snippet2test.png)

* My snippet 2 test passed✅

* Reviewed repo Snippet 1 test output(failed):
  
![their snippet 2 test output](images4/theirsnip2testr.png)

* Code change answer: 
Although my snippet 2 tester passed, there are still ways to improve the code. For tests with multiple parenthesis, it would be best to find the last closed parenthesis and updated the index of ```closeParen``` to that index.
***
  
## Snippet 3:

* What should be produced:
  
![snippet3actual](images4/snippet3actual.png)
    
* Test used for both my repo and reviewed repo: 
    
![snippet3test](images4/snippet3test.png)
   
* My snippet 3 test output(failed):
    
![mysnippet 3 test output](images4/mysnip3testr.png)
    
* Reviewed repo Snippet 1 test output(failed):
   
![their snippet 3 test output](images4/theirsnip3testr2.png)

* Code change answer: I believe that there is a small code change I could make that could read links with new lines. I could add an ```if``` statement that could check if there was a new line(using ```\n```) after ```nextCloseBracket``` or ```openParen```. 