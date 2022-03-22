## How to decide which breakpoints to use?

Deciding which breakpoints to use is a common thing. A lot of people will just look at common device sizes and target those and be done. While this works it's impossible to hit every device size. There are so many device sizes.

What you can do is almost combine two approaches. First look at when your layout starts to break. When you notice  your layout and content starts to break, then yoou can create a `media-query` around that size. Though this could get you starting to create a ton of different media queries because you want it to look at at every  size. then you can look at the common device sizes and see that not many devices would be at that size so you understand you don't have to create a ton of different media queries just one one thing. When you have around 7 different breakpoints, then it becomes really hard to change everything to make it  look properly. It's good to try to aim to have a lot of styles grouped under one break point.

## 100% Correct way todo breakpoints

While it is important to maintain to find where things are breaking, here is an article that explains and shows the most common device size and breakpoints:

[100% Correct Way Todo Breakpoints](https://www.freecodecamp.org/news/the-100-correct-way-to-do-css-breakpoints-88d6a5ba1862/)

The TL;DR Version:

* 600px
* 900px
* 1200px
* 1800px if you plan on giving people with giant monitors something special