# Day 6 - Review

This is mainly a review of what we have learned so far. So far we have learned:

* Using Percentages for widths
* Avoiding to set heights
* using max-width

While these aren't complicated, it is key to know these things to master creating responsive layouts.

## Why you shouldn't use ems for font-size

It is important to remember the difference between `em`'s and `rem`'s and the important thing to remember is that for `font-size` `em` looks at the  parent's `font-size`. This is important to remember because `em`'s is that they will compound on each other.

Here is a good video from Kevin Powell demoing this: [Why you shouldn't set font-sizes using em](https://www.youtube.com/watch?v=pautqDqa54I)

---

## A tale of width and max-width

An important thing to remember for the most part is that: If an element would render wider than what `max-width` says it can be, `max-width` wins.

[This CSS Tricks Article](https://css-tricks.com/tale-width-max-width/) explains and show's `width` and `max-width`.