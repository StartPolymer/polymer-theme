# Polymer Theme

Polymer Theme based on [BEM Methodology](http://getbem.com) and
[Material Design](http://www.google.com/design/spec/material-design/introduction.html) language.

For scaffolding Polymer apps use [Polymer Starter Kit](https://github.com/StartPolymer/polymer-starter-kit)
or [Polymer generator](https://github.com/yeoman/generator-polymer).

:sparkles: [DEMO](http://polymer-starter-kit.startpolymer.org) :sparkles:

## Features

- Based on [BEM (Block Element Modifier) Methodology](http://getbem.com)
 - Reusable CSS styles based on `class` attribute
 - Independent blocks and css selectors plus layer system makes your code reusable and modular
 - You don't need [calculating a selector's specificity](http://www.w3.org/TR/css3-selectors/#specificity)
- Using [Sass](http://sass-lang.com) CSS Preprocessor
- [Material Design typeface in CSS](http://materialdesignblog.com/material-design-typeface-in-css/)
 - Check out the [demo](http://polymer-starter-kit.startpolymer.org)
- [Roboto Font Combinations](https://github.com/StartPolymer/polymer-theme/wiki/Roboto-Font-Combinations)
- Based on [Material Design Color Palette](http://www.google.com/design/spec/style/color.html#color-color-palette)
 - Check out the [variables.scss](https://github.com/StartPolymer/polymer-theme/blob/master/sass/_variables.scss) and
 [material-colors.scss](https://github.com/StartPolymer/polymer-theme/blob/master/sass/modules/_material-colors.scss) module

## Installation

```sh
bower install polymer-theme --save
```

## Usage

### app.scss

```scss
$font-name-heading:       'roboto-slab';
$font-lang:               'en';
@import 'bower_components/polymer-theme/sass/base';

body {
  font-family: $font-body;

  /deep/ {
    h1,
    h2,
    h3 {
      font-family: $font-heading;
    }
  }
}

.polymer-theme {
  $color-name-primary:    'indigo';
  $color-name-secondary:  'pink';
  $color-name-text:       'grey';
  @import 'bower_components/polymer-theme/sass/variables';
  /deep/ {
    @import 'bower_components/polymer-theme/sass/blocks/all';
  }
}
```

### index.html

```html
<body class="polymer-theme">
```

## [Variables](https://github.com/StartPolymer/polymer-theme/blob/master/sass/_variables.scss)

### Material Design Colors

- [Link to module](https://github.com/StartPolymer/polymer-theme/blob/master/sass/modules/_material-colors.scss)

```scss
$color-name-primary:      'indigo';
$color-name-secondary:    'pink';
$color-name-text:         'grey';
```

### Roboto Font Combinations

- [Link to module](https://github.com/StartPolymer/polymer-theme/blob/master/sass/modules/_roboto-fonts.scss)

```scss
$font-name-heading:       'roboto-slab';
$font-lang:               'en';
```

## Contributing :+1:

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Make your changes
4. Run the tests, adding new ones for your own code if necessary
5. Commit your changes (`git commit -am 'Added some feature'`)
6. Push to the branch (`git push origin my-new-feature`)
7. Create new Pull Request

## [MIT License](https://github.com/StartPolymer/polymer-theme/blob/master/LICENSE)

Copyright (c) 2015 Start Polymer ([http://startpolymer.org](http://startpolymer.org))
