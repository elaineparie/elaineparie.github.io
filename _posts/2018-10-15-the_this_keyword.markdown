---
layout: post
title:      "The This Keyword"
date:       2018-10-15 12:23:22 +0000
permalink:  the_this_keyword
---


The value of this is based on the context in which the keyword is called. Outside of a function, this refers to the global object (a.k.a the window if in a browser). However, inside and object method, this refers to the object. Inside a standalone function or a callback function, this will be global or undefined. 

In the case of an arrow function, this is defined by its scope. They do not have their own scope. 

In other words, this refers to the context of where it is. 

We must also take into account the use of strict mode when calling this from insides of classes which will sometimes lead this to be undefined. 

One can alter the value of this using bind(), call() and apply() which control the invocation of the the function. Methods call() and apply() are used for immediate use while bind() returns a bound function that will execute later. 

The following examples of call(), apply(), and bind() are provided by codementor.io:

```
var obj = {name:"Niladri"};

var greeting = function(a,b,c){
    return "welcome "+this.name+" to "+a+" "+b+" in "+c;
};

console.log(greeting.call(obj,"Newtown","KOLKATA","WB"));
// returns output as welcome Niladri to Newtown KOLKATA in WB
```


Method apply() has a very similar effect with slightly different syntax:

~~~

```*var obj = {name:"Niladri"};


var greeting = function(a,b,c){
return "welcome "+this.name+" to "+a+" "+b+" in "+c;
};

// array of arguments to the actual function
var args = ["Newtown","KOLKATA","WB"];  
console.log("Output using .apply() below ")
console.log(greeting.apply(obj,args));

/ The output will be 
Output using .apply() below
welcome Niladri to Newtown KOLKATA in WB /*
```
 
 ~~~


When using bind(), you bind this to your context and can call the bound function later:

~~~

```
var obj = {name:"Niladri"};

var greeting = function(a,b,c){
    return "welcome "+this.name+" to "+a+" "+b+" in "+c;
};

//creates a bound function that has same body and parameters 
var bound = greeting.bind(obj); 


console.dir(bound); ///returns a function

console.log("Output using .bind() below ");

console.log(bound("Newtown","KOLKATA","WB")); //call the bound function

/* the output will be 
Output using .bind() below
welcome Niladri to Newtown KOLKATA in WB */
```

