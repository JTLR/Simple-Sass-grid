Simple Sass Grid
================

SSG is what it says on the tin, a simple responsive grid generated using Sass. 

## Features ##

- Support for columns across multiple breakpoints
- Customisable amount of columns, grid width, column size, column margin size, breakpoints and breakpoint names.
- Push (from left) classes across multiple breakpoints
- Show/hide classes across multiple breakpoints

## Usage ##

To set up an SSG grid you need to follow this convention:

``` html
<div class="grid">
	<div class="row">
		<div class="col small-12 large-18">
			Content
		</div>
		<div class="col small-12 large-6">
			Content
		</div>
	</div>
</div>
```

## Customisation ##

To change any aspect of the generated grid, change the variables in the `_setup.scss` file.

Currently you may only explicitly set either the `$column-width` or `$column-margin` variables.

## Browser support ##

SSG has been tested and works in Chrome, Firefox and IE9+ without any additional changes.

As the last `.col` element has its right hand margin removed via the `:last-child` pseudo selector, this won't work natively in IE7/8. To support IE7/8 simply add the class `last` to the last `.col` element in a row.

Bare in mind also that IE7/8 don't support media queries therefore each column will take its width from the class of the latest breakpoint. For example `large-16` will override `medium-20`.

## License ##

MIT