# Susy Bricks

Atomic CSS Classes for Susy <http://susy.oddbird.net/>


## About

Susy Bricks is a SCSS module for [Susy](https://github.com/oddbird/susy) <http://susy.oddbird.net/> that creates responsive, atomic CSS for Susy's grid system to make rapid prototyping easy.


## Credit

The prefix mixin comes from Buzzfeed's SOLID <http://solid.buzzfeed.com/>


## Installation

```
npm install susybricks
```

or if you'd like to just grab the repo
````
git clone git@github.com:seanblanton/susybricks.git
````


## Usage

Import the module 
```scss
@import "bricks/bricks";
````

Use the prefixes `.xs`, `.sm`, `.md`, and `.lg` in conjunction with susy's layout commands to quickly adjust layout. 
Susy Bricks supports 4 different Susy commands: `Span()`, `Last`, `Push`, and `Pull`

```html
<div class="box xs-span12 md-span6 lg-span3"> 
```

Update `/lib/settings.scss` to adjust the number of columns to fit your Susy layout and `$breakpoints` to meet your content needs. 
You can extend the number of columns and breakpoints as you see fit.

Example:
```scss
$susy-columns: 16; // Number of columns in susy grid


$breakpoints: (
  'xs': null, // always leave this at NULL
  'sm': 40rem, 
  'md': 64rem,
  'lg': 85rem,
  'xlg': 95rem,
);

```



## Authors

[Sean Blanton](http://www.sean-blanton.com)


---

[MIT license](LICENSE.md)
