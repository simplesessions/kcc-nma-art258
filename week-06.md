#### KCC NMA ART-258
# Week 06

## (Re-)Introducing JavaScript

JavaScript is used to add interactivity and DOM manipulation to the web. [The Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/JavaScript) (again, a great resource for everything on the web) dives a bit deeper on JavaScript's involvement in the web today.

### 6 Types of Data in JavaScript

- __`Number`__: a number. What else would this be?
- __`String`__: a way to write words within JavaScript
- __`Boolean`__: a value of either `true` or `false`
- __`Array`__: a simple, ordered collection of values, where each value is accessed by a numbered index. [More on Arrays](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
- __`Function`__: a command that you create that executes a command or series of commands that perform some action. [More on Functions](https://developer.mozilla.org/en-US/docs/Glossary/Function)
- __`Object`__: a collection of properties that relate to each other where these properties are represented with a key and a value. [More on Objects] (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)
  
	e.g. a Car could look like so:
  
	````
	var Car = {
		passengers: 2,
		wheels: 4,
		drive: function() {
			console.log("I am driving");
		}
	}
