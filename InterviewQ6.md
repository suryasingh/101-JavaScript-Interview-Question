##### 18. what is function hoisting in JavaScript? 

**Function Expression**

```javascript
 var foo = function foo(){ 
 	return 12; 
 }; 
```
> In JavaScript variable and functions are `hoisted`. Let's take function `hoisting` first. Basically, the JavaScript interpreter looks ahead to find all the variable declaration and hoists them to the top of the function where it's declared. For Example:

```javascript
 foo(); // Here foo is still undefined 
 var foo = function foo(){ 
 	return 12; 
 }; 
```
Above code behind the scene look something like below code: 

 ```javascript
   var foo = undefined;
      foo(); // Here foo is undefined 
  	   foo = function foo(){
  	      / Some code stuff
       }
 ```
 ```javascript
   var foo = undefined;
  	   foo = function foo(){
  	      / Some code stuff
       }
       foo(); // Now foo is defined here
 ```
  
 
 






