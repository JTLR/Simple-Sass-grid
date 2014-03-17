Simple-Sass-grid
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

## License ##

MIT