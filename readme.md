# ModularScale
## Compose your type to a scale

ModularScale is an scss file to make composing your type to a scale easy. It's just an automation of [Tim Browns’ (@nicewebtype)](https://twitter.com/nicewebtype) [Modular Scale](http://modularscale.com/), so be sure to [check out his presentation on the matter](http://vimeo.com/17079380) to really grasp what it's about (it just takes thirty minutes, and it's really worth it!).

### Workflow

1. Import the `modularscale.scss` file in your project

2. Assign your ideal body copy font-size (the pixel size at which your body copy looks best) in the `$font-size` variable **without** “px” (e.g. `$font-size: 18;`—default is 16)

3. Choose a scale by setting the `$scale` variable to `$perfect-fourth` | `$perfect-fifth` | `$golden-section` (default is `$perfect-fifth`. `$perfect-fourth` are more subtle increments in size, `$golden-section` are more drastic increments.)

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

	The `font-size()` mixin will set your font-size in rem's **with** a pixel fallback.

5. If you want, you can also use an “important number” for more variation in you scale. Again, check Tim Brown's presentation for more info on the subject.

	““If you want to mix font families, … adjust the sizes so that the x-heights aling.” - Thinking With Type

	So ideally, you would check which font size makes the x-height of your alternate font (e.g. the one you use for titles) match with the x-height of your body copy, and enter that as important number:

	e.g. `$important-number: 23;` (default is 0)

	Now you can access this scale through the variables

	1. `$ixxs`
	2. `$ixs`
	3. `$is`
	4. `$im`
	5. `$il`
	6. `$ixl`
	7. `$ixxl`
	8. `$ixxxl`
	9. `$ixxxxl`
	10. `$ixxxxxl`

	with the “i” standing for “important number.”

