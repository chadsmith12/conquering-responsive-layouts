# Deeper Dive Into Flex Box

This is deeper dive into flex box usin the following three part series from Kevin Powell: [Flexbox Tutorial](https://www.youtube.com/playlist?list=PL4-IK0AVhVjMSb9c06AjRlTpvxL3otpUd)

## Flexbox Containers

**Flex Properties**

* `flex-direction` - Defaults to row.  You can do `row-reverse` is like doing a `float: right`. Next is `column` which completely changes from `row`. This could be handy in media queries for responsive sites, to  go from `row`to `column`.

* `flex-wrap` - Defaults to `nowrap`. This means that items will be a single line. It's posible that the items get too small and they could spill out the side. You  can go to `wrap` and they will wrap around if they run out of room. With `nowrap` the `width` almost acts as if if it's a `max-width`.

* `flex-flow` -  shorthand for `flex-direction` and `flex-wrap`. So you can say: `row nowrap`.

* `justify-content` - Defaults to `flex-start`. `flex-end` will push everything to the  main.  `justify-content` works off the main axis. You can `center` things with `center`. There is also `space-between`

* `align-items` - Defaults to `stretch`. There is `flex-start` which pushes the item  all the way to the start. `flex-end` will  push the items all the down to  the end of the item. `align-items` always works on the cross axis. Which means for `row` it works off the vertical axis, and visa-versa for `column`.

* `align-content` - Has same properties has  `justify-content`. This only works with multi-lines of content. It works very similar to `justify-content` just that it has to have multi-lines and it does not work with `align-items`. 