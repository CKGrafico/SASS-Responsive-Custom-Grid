##SASS Grid

### ¿Why this?
- Has custom responsive. Normally the grid templates change to single column when you resize the browser, now you can add custom classes for change this.

```css
.three_quarters -> 75%
.half -> 50%
.third -> 33.33%
.fourth -> 25%
.hidden -> hide this element
```
```html
<div class="col_1-2 half">Col 1-2</div>
```
- Use SASS!!
Thanks to this you can only use necessary css.

```css
@include responsiveGrid(
	// Number of columns #default: 12
	//$max : 12,
	// Columns 1 to i #default: 1 2 3 4 5 6 7 8 9 10 11 12
	//$one-i: 1 2  4 5 7 9 10 12,
	// Columns i to max #default: 2 3 4 5 6 7 8 9 10 11
	//$i-max : 2 3 5 6 7 9 11
);
```

- And also it's easy customizable

##Example:

```html
<div class="grid">
	<div class="grid-row">
		<div class="col_1-1">Col 1-1</div>
	</div>
	<div class="grid-row">
		<div class="col_1-2 half">Col 1-2</div>
		<div class="col_1-2 half">Col 1-2</div>
	</div>
</div>
```
-----

Preview: http://ckgrafico.github.io/SASS-Responsive-Custom-Grid
