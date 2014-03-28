# 10grid Responsive CSS Layout

10grid is a very simple responsive CSS stylesheet inspired by https://github.com/dope/lemonade.  I wanted something that was the absolute bare-minimum that supports rapid hackability for basic websites, rather than using monsters like Bootstrap or Foundation which seemed crazy for a  tiny site.

Features:
* 10 column grid system using relatively-sized columns.
* Pre-built breakpoint for small screens that linearises the grid (also relatively-sized)
* Utility CSS classes for "smallOnly"/"notSmall" small-screen visibility

## Usage
* Set up the viewport to scale to width e.g. <meta name="viewport" content="initial-scale=1">
* Include 10grid.css in your HTML, e.g.  <link rel="stylesheet" href="10grid.css" />
* Add any other styles you want in your own style sheet and include as usual.
* Start writing easy responsive sites with the simple syntax.

The following snippet shows a row with 3 columns in the 2-6-2 formation.  Here we're using the "notSmall" class on the col-2 columns to hide them on small screens.
```html
<div class="row">
	<div class="col-2 notSmall">col-2</div>
	<div class="col-6">col-6</div>
	<div class="col-2 notSmall">col-2</div>
</div>
```
You dont have to "fill" the 10 column space, if you just wanted say a col-5 column and nothing else, you can do that too (the column will be left-aligned):
```html
<div class="row">
	<div class="col-5>col-5</div>
</div>
```
Please see the index.html page for a sample.
