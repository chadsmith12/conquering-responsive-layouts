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

---

## Flex Items

Flex items are the things inside of a flexbox. When you make something `display: flex` then everything becomes an item.

* `flex-grow` - Defaults to 0 and is a unitless number. If you put a 1, then it will take up all of the space it can. This determines how fast it should grow.
* `flex-shrink` - This is similar to `flex-row` but it deals with how fast it will shrink. A larger number here means that will show shrink faster than the others. It will work off the `flex-basis`.
* `flex-basis` - This is how much room you WANT it to take up, if it can. This acts as if an ideal width, but will get smaller if it can. If this is combined with a `flex-grow`  where it can grow. it will attempt to grow  if there is space it can take up.
* `order` - This allow you to control the order of things. This defaults to 0. So  this means if you give one thing an `order` of 1, then it means it actaully goes to the end. Giving it a negative value like -1  will pull it to the beginning. Order is good to use when going to mobile and  you don't like the way things are falling.
* `align-self` - Works similar to the `align-items` property, except that it is aligning only itself.
* `flex` -  This is the shorthand of combining all of `flex-grow`, `flex-shrink`, and `flex-bases` all onto one line. Example: `flex: 0 1 250px` would be a `flex-grow` of 0. A `flex-shrink` of 1 and a `flex-basis` of 250px.