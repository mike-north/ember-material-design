[![Build Status](https://travis-ci.org/mike1o1/ember-material-design.svg?branch=master)](https://travis-ci.org/mike1o1/ember-material-design)
[![Ember Observer Score](http://emberobserver.com/badges/ember-material-design.svg)](http://emberobserver.com/addons/ember-material-design)
[![Sauce Test Status](https://saucelabs.com/browser-matrix/ember_md.svg?auth=4224566d3e5343c119fbee3ab24f34c7)](https://saucelabs.com/u/ember_md)


# Ember-material-design

The **Ember Material Design** project is an implementation of Material Design in EmberJS. This project 
attempts to provide a set of reusable, well-tested and accessible UI components based on the Material Design system.

This project is as close to a reference implementation of [Angular Material](http://material.angularjs.org) as 
I could make it. Most of the credit for this work belongs to that team.


## Demo

Visit [Demo Page](http://mike1234.com/ember-material-design) to view the components in action.


## Installation

Install the ember-cli addon into project

```
$ ember install ember-material-design
```

This project uses SASS for compiling stylesheets. Import them into your styles.scss. 

```sass
@import "ember-material-design";
```
 
To use SASS, you will need to either install `broccoli-sass` or `ember-cli-sass`.

```
$ ember install ember-cli-sass
```

This project does not provide any vendor prefixes. It is highly recommended to use an autoprefixer. I prefer to use `ember-cli-autoprefixer`
which can be installed as an addon very easily.

```
$ ember install ember-cli-autoprefixer
```

Any variables you want to set should be set prior to importing the `ember-material-design` stylesheet.

For example, to change the `$primary` color:

```sass
$primary: 'red';

@import "ember-material-design";
```


## Fonts

By default, the `RobotoDraft` font is used from the Google Fonts api. To include this font, add the following line in the 
`<head>` section of your index page.

```html
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=RobotoDraft:300,400,500,700,400italic">
```

If you wish to use another font, overwrite the `$font-family` in a .scss file before your `@import "ember-material-design";`.
