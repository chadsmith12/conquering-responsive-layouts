# Day 1 -  Percentages and Avoiding Heights
Before you even add CSS you have a responsive website. It might not look very good but it is a response website. As soon as you start setting values that is where issues can start to rise


## Percentages vs. Fixed Widths
Default width for block-level elements, like `div` is 100%. It is important to note that this is a percentage. It will always be 100% of the parent, whatever the parent element is.

When you set a `width` to something like `900px` you lose your responsiveness, and then you end up creating a lot of different media queries to get rid of the horizontal scrolling and  it doesn't really look good. 

When you set a `width` to something like `80%` then it  will take up `80%` of the  parent. So this would end up creating an element that is `80%` of the viewport, if you think of the `body` as what the viewport is.