# Widths Generator

The `widths-generator` module is a **plugin for [inuitcss](http://inuitcss.com/)**.
This is a simple file that generates a series of helper classes to drop widths onto
elements such as grid systems.

It allow you to generate only the widths you need, as well as some extra proportions, like 16, 24...

This module **completely replace the default [`widths`](https://github.com/inuitcss/trumps.widths)
module** of inuitcss. So it's not necessary to load both the default `widths` module
and the `widths-generator` module.


## Installation

Install using Bower:

    $ bower install --save inuit-widths-generator


## Default options

inuitcss’ widths classes are available in one of two formats. The default format
is fraction-like, e.g.: `<div class="1/2">`.

The other available format is spoken-word, e.g. `<div class="one-half">`. Enable
this by predefining the `$inuit-use-fractions` feature switch, e.g.:

    $inuit-use-fractions:    false;
    @import "path/to/trumps.widths-generator";


## Define which widths you want to generate

By default it generate the same widths as the default `widths` inuitcss module.
But you can easily redefine which widths you need, e.g.: 

    $inuit-widths: 1, 2, 3, 12, 16;
