#### KCC NMA ART-258
# Week 02: Class: 02

## Class Notes

### Sites Shared

- [http://www.apple.com/iphone-6s/](http://www.apple.com/iphone-6s/)
  - Apple was and usually still is the standard for web design.
  - The effect with phones moving and falling down and rotating are accomplished with a combination of several technlogies:
	  - JavaScript: the browser senses where on the viewport the user is currently scrolling by looking at [scroll events](https://developer.mozilla.org/en-US/docs/Web/Events/scroll). When the user scrolls phones into view, they'll slightly rotate. A couple of them play videos.
	  - While the movement of the phones are triggered by the scoll position, their actual look is changed and styled via JavaScript and CSS Transforms [[1](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transforms/Using_CSS_transforms)] [[2](https://developer.mozilla.org/en-US/docs/Web/CSS/transform)]. CSS Transforms allow you to change certain visual properties of an element.
	  - It's hard to say, exactly how the transforms are animated without looking deeper, but there are posibilities that come to mind:
		  - JavaScript is used to apply CSS Transformation properties over time. This is the most likely scenario. Later in the semester, I'll be demonstrating how to transform CSS properties with JavaScript.
		  - CSS Transitions [[1](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions)] [[2](https://developer.mozilla.org/en-US/docs/Web/CSS/transition)]. Unlike transforms, transitions help to define how a CSS property changes between two states over a period of time. We'll also be learning more about CSS Transitions this semester.
		  - CSS Animations [[1](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations/Using_CSS_animations)] [[2](https://developer.mozilla.org/en-US/docs/Web/CSS/animation)] [[3](https://css-tricks.com/almanac/properties/a/animation/)]. CSS Animation is a more complex version of CSS Transitions that allows you more control over how you can define how CSS properties change between several states over time. You can also define other properties, like the direction in which the animation moves and how many times you want the animation to play.

--

### CSS Rules & Properties

- __`justify-content`__ - A flexbox-related property that controls the horizontal layout of a parent element that has the `display: flex` property.
- __`align-items`__ - A flexbox-related property that controls the vertical layout of a parent element that has the `display: flex` property.

This bears repeating: [read this guide on flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) if you haven't already.

--

### Terminology

- __clearing floats__ - Altthough we're utilizing flexbox a lot, there are still many instances you would use floats, or code that you will take over from someone else who has used floats for layout. In this case, always remember to clear your floats; this means that after using a `float` property on an element, there should be some property that comes after that which "clears" it by using the `clear` property. Read more: [All About Floats](https://css-tricks.com/all-about-floats/)
	- There is a trick that allows you to *self-clear* an element called *clearfix*. As demonstrated in class, if you have a parent element where its two child elements are both floated, the parent element doesn't know about its own layout because nothing has cleared the floats. Using a [clearfix hack (scroll to the bottom of the article)](https://css-tricks.com/snippets/css/clear-fix/) on the parent element allows you to clear the element within your CSS. Ask me for help if you need assistance on this.


--

### Other Useful Links

- Filler Text
	- [Lorem Ipsum](http://lipsum.com/)
	- [Bacon Ipsum](http://baconipsum.com/)
 	- [Hipster Ipsum](http://hipsum.co/)
 	- Note: there are a ton of filler text sites out there. Use any one that you want!
- Stock Photos
	- [Free Stock Photos That Don't Suck @ Medium](https://medium.com/@dustin/stock-photos-that-dont-suck-62ae4bcbe01b#.42zycsd91)
- Typography
	- [CSS Typography: The Basics](http://sixrevisions.com/css/css-typography-01/)

--

### Class Exercises

- [Codepen: Just Do It](http://codepen.io/simplesessions/pen/PGoKKG)

#### Suggested Exercises

- [Fork the Codepen example](https://blog.codepen.io/documentation/features/forks/) above an experiment with different ways to change up the layout:
	- Change the colors, type, background, etc. to match something that's a little more... visually pleasing.
	- Make two rows of navigation links that stack on top of each other, but still line up vertically with the logo.
	- Expand on the aside, and try and create more content. See what could possibly fit in there.

--

