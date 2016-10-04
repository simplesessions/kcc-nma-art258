#### KCC NMA ART-258
# Week 05

_Note: I'll be doing class notes based on the week from here on out instead of breaking them out by day._

## Disecting the Project Starter Files

[ART-258 Project Starter Git Repo](https://github.com/simplesessions/kcc-nma-art258-starter)

_Note: Since the original discussion in class, there may have been changes to the files discussed here. The most up-to-date notes will be displayed with the repo_

----

__`src`__ - where you'll be editing all your files for your projects. Within this, you'll have the following folders/files:

- `images` - the folder where all your image assets go.
- `scss` - your Sass files, which are transformed into CSS files.
- `index.html` - your main HTML starter file.

__`.gitignore`__ - a "dot file" (invisible file) that holds a list of files and folders that will not be added to your project as you check in your changes. Among the list is the `node_modules` folder, which you should never check in.

__`.stylelintrc.json`__ - configures the linter for CSS files. You can [read more about what linting is](https://en.wikipedia.org/wiki/Lint_%28software%29) on your own, but linting is basically a way to enforce propper formatting and basic error-checking within your code. In this case, we're using a program called [stylelint](http://stylelint.io), installed with when you run `npm install`, to output any problems with your stylesheets to the CLI. This file is a configuration file to help `stylelint` know which rules to pay attention to.

__`README.md`__ - what you see on GitHub that describes the project. It's written in a format called [Markdown](https://help.github.com/articles/basic-writing-and-formatting-syntax/).

__`gulpfile.js`__ - controls [gulp](http://gulpjs.com), the task runner that we're using to run all the tasks that "build" our projects.

## Sass Introduction

[Sass](http://sass-lang.com) is a preprocessor ([What's is a CSS Preprocessor?](https://drupalize.me/videos/what-css-preprocessor?p=1175)) that transforms code written in Sass to CSS.

Using the [Sass Basics Guide](http://sass-lang.com/guide) as a basis, we've gone over the following concepts so far in class:

- variables
- nesting
- partials
- import

We'll try and incorporate other concepts during our projects, but read ahead to learn more about other concepts in the basics guide like `mixins` and `extends`. 

Feel free to search for more tutorials about Sass – there are a lot out there – but, here are some more useful links to continue to learn more about Sass:

- [http://alistapart.com/article/why-sass](http://alistapart.com/article/why-sass)
- [https://css-tricks.com/sass-style-guide/](https://css-tricks.com/sass-style-guide/)
- [https://css-tricks.com/the-sass-ampersand/](https://css-tricks.com/the-sass-ampersand/)

