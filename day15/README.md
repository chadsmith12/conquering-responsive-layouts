# Day 15 - Intro To Media Queries

## Media Query Basics

Media Queries let us add new styles or override specific styles under certain  conditions.

The media query syntax is followed as:

```css
@media() {

}
```
You can inclue a `media-type`, but you don't have to.

A popular one is screen size. So for example you can do `min-width` to say "it matches this width or bigger. Example:

```css
/*600 pixels or bigger*/
@media(min-width: 600px) {

}

/*600 pixels or smaller*/
@media(max-width: 600px) {

}

/*From 600 pixels - 900 pixels*/
@media(min-width: 600px) and (max-width: 900px) {

}
```

It's important to note that `media-query` is only going to override the property that you change. It will keep any other styles already applied.

Also when writing media queries, you should write them from smallest to biggest so that way they can override each other when going up in screen sizes.