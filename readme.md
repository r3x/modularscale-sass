# Sassy Modular Scale
#### Put down the calculator and let Sass do the work.

# Usage and Installation

Sass Modular Scale is written in Sass and requires Sass to be used. Visit [sass-lang.com](http://sass-lang.com) to learn more and install.

* Copy either `stylesheets/_modular-scale.sass` or `stylesheets/_modular-scale.scss` into your project
* Import the file into your Sass stylesheet to access the mixins and functions

Sassy Modular Scale can be used as a function, mixin or a mixin that generates a range of classes to `@extend`.

Examples using the Sass syntax:

    // Use as a function. Fill in the multiple, base-size, and ratio
    height: modular-scale(7, 14px, $golden)
    
    // Use as a mixin. Fill in the property, multiple, base-size, and ratio
    +modular-scale(line-height, 1, 14px, $golden)
    
    // This method will generate a range of classes to `@extend`
    +modular-scale-classes(6)

    [role="main"]
      h1
        @extend .ms-2
      h2
        @extend .ms-1
      h3
        @extend .ms-0

Examples using the SCSS syntax:

    // Use as a function. Fill in the multiple, base-size, and ratio
    height: modular-scale(7, 14px, $golden);
    
    // Use as a mixin. Fill in the property, multiple, base-size, and ratio
    @include modular-scale(line-height, 1, 14px, $golden);

    // This method will generate a range of classes to `@extend`
    @ionclude modular-scale-classes(6);

    [role="main"] {
      h1 { @extend .ms-2; }
      h2 { @extend .ms-1; }
      h3 { @extend .ms-0; }
    }

# Ratios

Below is a list of Ratios to choose from. By default, the variable `$ratio` is set to `$golden`.

* $golden: 1.618
* $octave: 2 / 1
* $major-seventh: 15 / 8
* $minor-seventh: 16 / 9
* $major-sixth: 5 / 3
* $minor-sixth: 8 / 5
* $fifth: 3 / 2
* $fourth: 4 / 3
* $major-third: 5 / 4
* $minor-third: 6 / 5
* $major-second: 9 / 8
* $minor-second: 16 / 15

# Credits

#### Sass mixin by Scott Kellum

* [https://github.com/scottkellum/modular-scale](https://github.com/scottkellum/modular-scale)
* [@scottkellum](http://twitter.com/scottkellum)

#### Adapted from modularscale.com by Tim Brown

* [http://modularscale.com/](http://modularscale.com/)
* [@nicewebtype](http://twitter.com/nicewebtype)

#### Related link:

* [http://alistapart.com/articles/more-meaningful-typography/](http://alistapart.com/articles/more-meaningful-typography/)

#### Additional credit to Robert Bringhurst

* The Elements of Typographic Style (Chapter 8: Shaping the page)
