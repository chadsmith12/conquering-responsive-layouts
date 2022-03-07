# Day 1 -  Percentages and Avoiding Heights

Before you even add CSS you have a responsive website. It might not look very good but it is a response website. As soon as you start setting values that is where issues can start to rise


## Percentages vs. Fixed Widths

Default width for block-level elements, like `div` is 100%. It is important to note that this is a percentage. It will always be 100% of the parent, whatever the parent element is.

When you set a `width` to something like `900px` you lose your responsiveness, and then you end up creating a lot of different media queries to get rid of the horizontal scrolling and  it doesn't really look good. 

When you set a `width` to something like `80%` then it  will take up `80%` of the  parent. So this would end up creating an element that is `80%` of the viewport, if you think of the `body` as what the viewport is.

## Percentages on the Child

Again, a common thing is to set a fixed width on a child element, and it looks ok on some screen sizes, but then on smaller devices it can start to overflow the parent. This can lead people to say this is CSS's fault, but this is a feature. CSS by default will attempt to make sure you don't lose information and will create the horizontal scroll bar to make sure you can scroll to see the content. 

When you set a percentage on a child element, it's  important to remember the percentage is always based on the parent element. So if the child element is `50%` then it is going to be `50%` of the parent element. So if the parent gets bigger, so will the child, and the same thing if it gets smaller.

Later on you will see that you don't even have to set a width on the child and that you don't always have to be setting one everytime.

## Why it's a good idea to avoid Heights
A general suggestion is that if you have to give something a height, don't. Heights can cause a lot of problems. An example of this is you give something a height because you want it to look a certain  way, then on certain devices the content starts to overflow it's container.

When you do need it to take up a certain amount then you can use padding.