# 13grid

A 13 column grid.

[[https://github.com/jmz7v/13grid/blob/master/images/13Grid.png|alt=13grid]]

## WHY?

Because none of the current 12 column grids satisfies me. I have used Bootstrap, Foundation, Pure and Toast and none of them have really convinced me.

I’m not sure if this is the first open source 13 grid column, I started it at school without internet using Sketch and haven’t stopped since. I don’t want to Google if another one already exists.

### To-Do

- Docs for usage


## 13 columns

I haven’t really used the 1/12 unit ever, so, I am dropping it or at least, dropping the 1/13.

I love centered stuff and 12 column grids didn’t satisfied me. I sketched a 13 column one to use one as a center and put in a lot of whitespace.

We are talking about a 30px FIXED gutter.

The standard size for the whole grid is 960px.

## The containers

### The Unit

The unit is also the gutter. There are 13 units in 13grid. Woah.

Default width @ 960px: 60px

Percentage width: 6.25%

### The One

Used for full content width, it’ll leave a unit of space at each side.

Default width @ 960px: 840px

Percentage width: 87.5%

### The Half

Kind of half the One.

Default width @ 960px: 390px

Percentage width: 40.625%

### The Third

Kind of a third of the One.

Default width @ 960px: 240px

Percentage width: 25%

### The Fourth

Kind of a fourth of the One.

Default width @ 960px: 165px

Percentage width: 17.1875%

### The Sixth

Kind of a sixth of the One.

Default width @ 960px: 90px

Percentage width: 9.375%

### The Two Thirds

Kind of 2 one thirds.

Default width @ 960px: 540px

Percentage width: 56.625% — Magic number may be?


## Usage

### Variables

Modify this to fit your needs

```sass
$content-max-width: 960px; // From Odyssey.scss
$side-padding: 15px;
$gutter: 6.25%;
$margin-between-rows: 6.25%;
$query-mobile: 600px;
$query-desktop: 920px;

```

### Responsive Classes

```css
[only-mobile] { /* Shows this content only in mobile */ }
[only-tablet] { /* Shows this content only in tablet */ }
[only-desktop] { /* Shows this content only in desktop */ }

[hidden-mobile] { /* Hides this content only in mobile */ }
[hidden-tablet] { /* Hides this content only in tablet */ }
[hidden-desktop] { /* Hides this content only in desktop */ }
```

Please note that tablet size is between the mobile and desktop, taken from it’s variables.

To add one of the previous classes add the markup to your HTML element like this
```html
<div class="myDiv" only-mobile>
	<p>Only visible in mobile</p>
</div>
```



## Acknowledgements

13grid was built on top of [Normalize.css](https://github.com/necolas/normalize.css/) by Nicolas Gallagher. 

13grid uses and it was planned to use alongside [Odyssey.css](https://github.com/Jmz7v/Odyssey.scss) by Julio Montaño. 

13grid was designed in [Sketch](http://bohemiancoding.com/sketch/).

13grid uses [SASS](http://sass-lang.com). The compiled version of 13grid is always up-to-date and ready to use.
