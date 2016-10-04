#### KCC NMA ART-258
# Week 06

## (Re-)Introducing JavaScript

JavaScript is used to add interactivity and DOM manipulation to the web. [The Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/JavaScript) (again, a great resource for everything on the web) dives a bit deeper on JavaScript's involvement in the web today.

More: [A Reintroduction to JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript)

### Operators

- __`=`: assign__ - assign a value in JavaScript from the right-hand side to the left-hand side. This not not mean "equals".

		var fruit = "orange"

- __`===`: equality__ - compare two statements with each other.

		fruit === "orange"			// true
		4 === 2						// false
		fruit === "banana"			// false
		3 === 3						// true

- __`+`: add or concatenate__

		4 + 7 + 8					// 19
		
		var name = "Charles"
		"Hello there, " + name		// "Hello there, Charles"

### 6 Types of Data in JavaScript

- __`Number`__: a number. What else would this be?
- __`String`__: a way to write words within JavaScript
- __`Boolean`__: a value of either `true` or `false`
- __`Array`__: a simple, ordered collection of values, where each value is accessed by a numbered index, starting with `0`. [More on Arrays](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

	e.g. an array of fruits:
	
	````javascript
	var fruits = ['apple', 'banana', 'orange']
	fruits[1]                 // "banana"
	fruits.push('grapes')     // ["apple", "banana", "orange", "grapes"]
	fruits[3]                 // "grapes"
	fruits.pop()              // ["apple", "banana", "orange"]
	fruits[3]                 // undefined
	fruits.unshift('prune')   // ['prune', "apple", "banana", "orange"]
	fruits.shift              // ["apple", "banana", "orange"]
	````

- __`Function`__: a command that you create that executes a command or series of commands that perform some action. [More on Functions](https://developer.mozilla.org/en-US/docs/Glossary/Function) and [More Function Explanations & Examples](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)
- __`Object`__: a collection of properties that relate to each other where these properties are represented with a key and a value. [More on Objects] (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)
  
	e.g. a Car could look like so:
  
	````javascript
	var Car = {
		passengers: 2,
		wheels: 4,
		drive: function() {
			console.log("I am driving")
		}
	}
	````

### Conditionals

Conditionals are used to control the flow of your script.

````javascript
	var minAge = 18
	var maxAge = 36
	var age = 16
 	if (age < minAge) {
 		console.log("Take a hike, kiddo, you're way too young!")
 	} else if (age > maxAge) {
 		console.log("You're a little older than our target demographic")
 	} else {
 		console.log("You're just the right age for us to serve you our ad!")
 	}
````

## jQuery

[jQuery](http://jquery.com) is a JavaScript library used to make certain parts of JavaScript easier, such as selecting elements within the DOM using CSS selector syntax.

More:

- [The Offical jQuery API Documentation](http://api.jquery.com)
- [The jQuery Learning Center](http://learn.jquery.com)
