# Sass boilerplate library

This is a boilerplate project containing the basic Sass styling code to get a project up and running.

Its structure is based on the SMACSS and 7-1 architecture patterns and it contains the basic code to get up and running with breakpoints, typography, colours and other core elements.

Many of the ideas are combinations of various other ideas with some enhancements.  I have tried to list all sources in the acknowledgements section.
It follows as many of the latest best practices as possible including atomic CSS, BEM, low selector specificity, good vertical rhythm, single direction margins etc.

This is not a library of awesome design ideas.  The colours etc. are for demonstration purposes only.  The breakpoints, font-sizing and margins etc. are valid and could be used although you will probably want to swap them out for something to fit with your own design.

If vertical rhythm and modular type scales are new to you then these are some good articles to read:
* [Modular type scale]( http://www.modularscale.com/?1&em&1.5&web&text )
* [Vertical rhythm](https://drewish.com/tools/vertical-rhythm/ )
* [Baseline grid](http://alistapart.com/article/settingtypeontheweb )
* [Putting it all together in code](https://scotch.io/tutorials/aesthetic-sass-3-typography-and-vertical-rhythm)

This project is work in progress and will forever stay that way as new concepts appear and best practice changes.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine.  All documentation is contained within the files themselves.  It can be read directly but a nicer way is to run it through [SassDoc](http://sassdoc.com/)

### Component based architecture

If you are using a component based architecture then this layout will fit in well to the structure. e.g. Vue or React.  The main app should include the general CSS build as main.css and each component can include only the required CSS for that component and if required, also scope it to that component.  The default included here has all components included in the main CSS file.  To support a component structure then remove the components from being included in the main CSS and include the individual component Sass files in each component.  They will then also need to import the combined abstracts file.

### Prerequisites

This project is written in Sass and so you will need a way of building Sass.
All the tools I have used are run using Node and Gulp although you can use anything that can compile Sass (.scss style). I am using gulp-sass.
[How to install and use gulp-sass](https://www.npmjs.com/package/gulp-sass)

## Authors

* **Jason Harris** - *Initial work* - [JayyajGH](https://github.com/JayyajGH)

See also the list of [contributors](https://github.com/JayyajGH/Sass-Boilerplate/graphs/contributors) who participated in this project.

## Contributing

Please read [CONTRIBUTING.md](https://github.com/JayyajGH/Sass-Boilerplate/blob/master/CONTRIBUTING.md) for details on the code of conduct, and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/JayyajGH/Sass-Boilerplate/blob/master/licence.md) file for details

## Acknowledgements

The structure of the boilerplate is based on two main patterns:
* [SMACSS](https://smacss.com/)
* [Sass Guidelines 7-1 pattern](https://sass-guidelin.es/#architecture)

The colour palette ideas were formed from these articles:
* [Using maps for setting up the colour palette](https://scotch.io/tutorials/aesthetic-sass-2-colors)
* [Using maps for setting the tone of the palette](http://erskinedesign.com/blog/friendlier-colour-names-sass-maps)

The initial idea for using Sass maps for breakpoints came from here:
* [Responsive breakpoints](https://www.sitepoint.com/managing-responsive-breakpoints-sass)

 Should we use pixels, rems or ems?  Hint:
 * Never use pixels
 * Use rems for sizing and spacing
 * Use ems for media queries
 * [Should we use pixels, rems or ems?](http://engageinteractive.co.uk/blog/em-vs-rem-vs-px)

Using utility classes:
* [The role of utility classes](http://davidtheclark.com/on-utility-classes/)
* [Namespaces for utility classes](https://csswizardry.com/2015/03/more-transparent-ui-code-with-namespaces/)

Using single direction margins:
* [Single direction margins](https://csswizardry.com/2012/06/single-direction-margin-declarations/)

Some static code analysis tools I've used are:
* [Sass linter](https://www.npmjs.com/package/sass-lint)
* [Stylesheet analysis tool - Parker](https://github.com/katiefenn/parker)
