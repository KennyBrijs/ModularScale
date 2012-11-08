# ModularScale
## Compose your type to a scale

ModularScale is an scss file to make composing your type to a scale easy. It's just an automation of [Tim Browns’ (@nicewebtype)](https://twitter.com/nicewebtype) [Modular Scale](http://modularscale.com/), so be sure to [check out his presentation on the matter](http://vimeo.com/17079380) to really grasp what it's about (it just takes thirty minutes, and it's really worth it!).

### Workflow

1. Import the file

2. Set your body copy font-size in the `$font-size` variable (default is 16)

3. Choose a scale by setting te `$scale` variable to `$perfect-fourth` | `$perfect-fifth` | `$golden-section` (default is `$perfect-fifth`. `$perfect-fourth` are more subtle increments in size, `$golden-section` are more drastic increments.)

4. Set your type using the the `font-size()` mixin with `$xxs` to `$xxxxxl` variables (e.g. `h1{ @include font-size($xxl);}`) (`$s` is default size for body copy)

	1. `$xxs`
	2. `$xs`
	3. `$s`
	4. `$m`
	5. `$l`
	6. `$xl`
	7. `$xxl`
	8. `$xxxl`
	9. `$xxxxl`
	10. `$xxxxxl`
