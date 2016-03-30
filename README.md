# pickadate

The mobile-friendly, responsive, and lightweight jQuery date & time input picker.

[![build status: master](https://img.shields.io/travis/blacklane/pickadate.js/master.svg?style=flat-square)](https://travis-ci.org/blacklane/pickadate.js) <sup>[`master`](https://github.com/blacklane/pickadate.js/)</sup>
[![build status: dev](https://img.shields.io/travis/blacklane/pickadate.js/dev.svg?style=flat-square)](https://travis-ci.org/blacklane/pickadate.js) <sup>[`dev`](https://github.com/blacklane/pickadate.js/tree/dev)</sup>
[![dependencies status](https://img.shields.io/david/blacklane/pickadate.js/master.svg?style=flat-square)](https://david-dm.org/blacklane/pickadate.js)
[![dev dependencies status](https://img.shields.io/david/dev/blacklane/pickadate.js/master.svg?style=flat-square)](https://david-dm.org/blacklane/pickadate.js#info=devDependencies)


#### To get started, check out the:

[Homepage](http://amsul.ca/pickadate.js) - [Date picker](http://amsul.ca/pickadate.js/date) - [Time picker](http://amsul.ca/pickadate.js/time) - [API](http://amsul.ca/pickadate.js/api)


#### To get it:

[Download the latest stable build](https://github.com/amsul/pickadate.js/archive/master.zip)

*or*

`git clone git://github.com/amsul/pickadate.js.git`

*or*

`bower install pickadate`




<br>
## Library files

The `lib` folder includes the library files with a `compressed` folder containing the minified counter-parts. These files are minified using [Grunt](#building-with-grunt).

### Pickers

There are three picker files:

* `picker.js` The core file (required before any other picker)
* `picker.date.js` The date picker
* `picker.time.js` The time picker

_To support old browsers, namely IE8, **also include** the `legacy.js` file._


### Themes

All themes are [generated using LESS](#less-styling) and compiled from the `lib/themes-source` folder into the `lib/themes` folder.

There are two themes:

* `default.css` The default modal-style theme
* `classic.css` The classic dropdown-style theme

Based on the theme, pick the relevant picker styles:

* `default.date.css` and `default.time.css` when using the default theme
* `classic.date.css` and `classic.time.css` when using the classic theme

__**__ For languages with text flowing from right-to-left, also include the `rtl.css` stylesheet.


### Translations

The translations live in the `lib/translations` folder. There are currently [43 language translations](https://github.com/amsul/pickadate.js/tree/master/lib/translations) included.




<br>
## Building with Grunt

[Grunt](http://gruntjs.com/) `~0.4.5` is used to build the project files. To get started, clone the project and then run:

- `npm install` to get the required node modules.
- `grunt test --verbose` to confirm you have all the dependencies.


Type out `grunt --help` to see a list of all the tasks available. The generally used tasks are:

- `grunt develop` compiles the LESS files and watches for any source changes.
- `grunt package` compiles and then minifies the source files.
- `grunt test` tests the entire package.




<br>
<a name="less-styling"></a>
## Styling with LESS

The picker themes are built using [LESS](http://lesscss.org/) with Grunt. To customize the CSS output, read the `_variables.less` file in the `lib/themes-source` folder. You can specify:

- colors for the theme,
- sizes for the picker,
- media-query breakpoints,
- and a whole bunch of other stuff.


Make sure to run the `grunt develop` task before making any changes to compile it into CSS.



<br>
## Versioning

To maintain consistency in the sort of changes to expect with version bumps, [Semantic Versioning guidelines](http://semver.org/) is followed as closely as possible:

`<major>.<minor>.<patch>`

Constructed as such:

- `major`: breaks backward compatibility (resets the `minor` and `patch`)
- `minor`: new additions with backward compatibility (resets the `patch`)
- `patch`: bug fixes and misc changes

If a version bump is due, make sure to update the version with a project-wide search and replace.





<br>
## Bugs

Before opening a new issue, please search the existing [Issues](https://github.com/amsul/pickadate.js/issues) for anything similar – there might already be an answer to your problem. You might also wanna check out the [Contributing](https://github.com/amsul/pickadate.js/blob/gh-pages/CONTRIBUTING.md) guide.





<br>
## Contributing

Before contributing any code to the project, please take a look at the [Contributing](https://github.com/amsul/pickadate.js/blob/gh-pages/CONTRIBUTING.md) guide.

If there’s anything you’d like to discuss, we like to hang out on Gitter.

[![Gitter](https://badges.gitter.im/Join Chat.svg)](https://gitter.im/amsul/pickadate.js)





<br>
## Support

If you find this library useful and would like to see further development, consider [supporting it](http://selz.co/1g80kCZ).





<br><br>

---

© 2014 [Amsul](http://twitter.com/amsul_)

Licensed under [MIT](http://amsul.ca/MIT)
