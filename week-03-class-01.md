#### KCC NMA ART-258
# Week 03: Class: 01

## Sites Shared

[Abstractions](http://abstractions.io) - Cool conference site.

- We'll come back to the site later to talk about the subtle animation done to the bushes as you scroll down the page.

## Terminology

__Sass__ - Sass (Symantically Awesome Stylesheets) is a technology called a _preprocessor_ made up of several libraries and a code compiler that transforms Sass code into CSS code. Sass has many advantages over vanilla (normal) CSS, including variables, mixins, and more. The best way to use Sass right now is through a Codepen pen.

- [Sass Home](http://sass-lang.com)
- [Sass Basics](http://sass-lang.com/guide)
- [Using Preprocessors in Codepen](https://blog.codepen.io/documentation/editor/using-css-preprocessors/)
- [Class Exercise: Small Example Using Jade & Sass](http://codepen.io/simplesessions/pen/JRdoJa)

_NOTE_: Although I introduced Sass in class, we will not employ it any further within our [projects](https://github.com/simplesessions/kcc-nma-art258-projects) until the second project.

__Media Queries__ - CSS code that will allow you to apply CSS rules based on viewport size creiteria. (See below for a basic example of how to do this).

- [http://mediaqueri.es/](http://mediaqueri.es/)
- [7 Habits of Highly Effective Media Queries by Brad Frost](http://bradfrost.com/blog/post/7-habits-of-highly-effective-media-queries/)

__Breakpoint__ - the part of your CSS design in which the design breaks, or changes, due to a Media Query. For example, if you have a Media Query as such: `@media screen and (min-width: 640px)`, you would refer to there being a breakpoint at 640px.

__Responsive Web Design__ - a design and coding methodology that employs the use of Media Queries to affect the design of elements the layout based on the size of the viewport.

- [Responsive Web Design by Ethan Marcotte @ A List Apart](http://alistapart.com/article/responsive-web-design)

__Mobile First__ - a design, content, and coding strategy that encourages creators of websites to approach the design of sites starting from a small device screen. While you nail down areas of the design at a smaller size, expanding the size of the viewport will reveal areas in which to add breakpoints and adjust the design.

- [Mobile First by Luke W](http://www.lukew.com/ff/entry.asp?933)
- [Suggested Reading – Mobile First: The Book by Luke W @ A Book Apart](https://abookapart.com/products/mobile-first)

## Class Exercises

[Layout Challenge: The Art of Designing With Heart](https://m.signalvnoise.com/the-art-of-designing-with-heart-f5dc4df21697)

[My Codepen Example from Class](http://codepen.io/simplesessions/pen/XjbJxY)

#### Media Queries CSS Code Sample

    p {
      padding: 1rem;
      font-size: .7rem;
      background: #009999;
      color: white;
    }

    @media screen and (min-width: 500px) {
      p {
        background: #990000;
        font-size: 1.2rem;
      }
    }
