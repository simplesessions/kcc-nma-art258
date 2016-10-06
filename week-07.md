#### KCC NMA ART-258
# Week 07

## More on JavaScript

Last week, we explored the different types within JavaScript. This week, we're learning a couple more jQuery concepts before putting our skills into practice in class.

### First, a Note on Documentation

The key to really getting to know how JavaScript works is to be able to read the documentation with anything that you use. The good and the bad thing about the open web is that, while there's lots of good documentation out there, especially for popular technologies and code libraries that people use, not a lot of documentation is read the same. Getting used to the terms and vocabulary that we go over in class will help to identify how to put the documentation to use.

### on JavaScript and jQuery

To reiterate, jQuery is a _JavaScript library_ that we use to help us write JavaScript code in a way that's both easier to use and understand. Remember, anything that looks like a `$()` in this class will refer to a jQuery function. These jQuery functions expect you to pass in a `String` made up of a `CSS Selector` as an argument. The jQuery function will `return` all the `Elements` that match, and you can call various other jQuery functions on the collection it returns.

It's also important to denote the difference between plain JavaScript and jQuery, as we'll be using both to get our work done. Again, look for pieces of code that use `$()`.

Brush up on JavaScript at the [Mozilla Developer Network](https://developer.mozilla.org/en-US/). I'm going to constantly repost this link, since it has a ton of great documentation and tutorials on learning JavaScript.

#### Learn more on jQuery:

- [Interactive jQuery Tutorial](http://try.jquery.com)
- [jQuery Documentation](http://api.jquery.com)

## JavaScript Concepts Discussed

- __`this`__ - the concept of `this` was discussed last class, but bears repeating. `this`, when used in certain contexts, refers to the current item you're working with. During this course, we've used `this` to refer to the current item when `iterating` over a collection of items in jQuery with `.each()`.

## jQuery Functions Discussed

- __`.each()`__ - iterates over the collection of items you've selected, and allows you to perform an action on each item.

	[Documentation for .each()](https://api.jquery.com/each/)


## Class Exercise #1 - [Codepen](http://codepen.io/simplesessions/pen/ZpvEyo)

In this exercise, we got used to using `.each()` to iterate over our collection of `<li>` elements. By iterating over each element, we were able to get each element's `innerHTML` property, change it to lower case with [`String.toLowerCase()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/toLowerCase), and were able to set this new value we've created as the element's [`className`](https://developer.mozilla.org/en-US/docs/Web/API/Element/className).

## Class Exercise #2 - [Codepen](http://codepen.io/simplesessions/pen/jrYEPK)

The purpose of this exercise was to have you guys get used to implementing [slick](https://kenwheeler.github.io/slick/), a jQuery carousel/slider library, on your own.

This involved the following skills:

- using jQuery, and identifying how jQuery works on a basic level, as well as how it interacts with a third-party library
- being able to interpret documentation for JavaScript libraries
- getting used to using [CDNs](https://en.wikipedia.org/wiki/Content_delivery_network) to load files needed for your library to [run as external resources in your Codepen pen](https://blog.codepen.io/documentation/editor/adding-external-resources/)
- using a JavaScript object as a way to configure your plugin, as this is a very common method for library/plugin configuration