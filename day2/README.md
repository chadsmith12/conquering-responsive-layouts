# Getting Familiar With Relative Units

## em

For `em` if you set a font size using  `em`s, then it will be in relation to that  elements parent. Exampe you set the parent's font size to be be 16px (usually browser default), and then set the childs font size to be `2.5em` then it would  be 2.5x the size of the parent. So It would be about 40.

Important thing about `em` is that it compounds. So if you set the parent to be `2.5em` and the child to be `2em` then it will compound up. The first will be 2.5 * 16, then the `2em` will be compounded off that.

Looking at the parent only happens for font sizes though.  If you use `em` for something like margin or padding, then  it actually just looks at that elements font size.

## rem

For `rem` it is similar, but `rem` was actually invented to fix the whole  compounding  problem that `em` has. What `rem` really stands for is "root em." It will look at the `html` root font size only. It  won't look at the body, just look at the root element.

While for `em` the margin and padding looks at the current element, `rem` will ALWAYS look at the root.  It is not variable, while  `em` is  variable.

