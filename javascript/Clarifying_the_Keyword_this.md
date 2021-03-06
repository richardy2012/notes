## JavaScript: Clarifying the Keyword ‘this’
> 
> The keyword ‘this’ holds a value and is bound to another object. It can be one of the most confusing subjects in JavaScript. It doesn’t have to be if you follow this simple rule:
The keyword ‘this’ is bound dynamically to the object found to the left of the ‘.’ at call time.
``` 
person={
	location:'SF',
        locate:function(){
		alert(this.location)
	}
  }
  person.location;
  person.locate
``` 
> 
> Call time is when a set of parenthesis () begins the execution of our function. In our case ”person” is to the left of the ‘”.’” at call time. So in the example above, ‘this’ refers to our object person.
> 
### There are three exceptions to the above.
 1) When there is no ‘.’ the keyword ‘this’ is bound to the global object window.
 2) When you use call and apply, you get to decide what ‘this’ is bound to.
 3) When you use the keyword new to create a new instance from a constructor, the keyword ‘this’ refers to the newly generated instance.
> 
> Special shout out to Marcus who’s a software engineer at Twitter and curriculum designer at Catalyst Class for teaching me how simple the keyword ‘this’  is. All credit goes to him.
