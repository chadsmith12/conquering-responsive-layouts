# Flexbox Basics

Flexbox is a quick way to lay things out. Naturally flexbox works in rows.

To enable flexbox you use the CSS Property: `display: flex`.  This will by default create a row flexbox container. This is by default a `flex-direction: row`. This means all the direct children become columns and forcing them next to each other.

The direct children of a flex container are the flex items. By default a flex item is trying to shrink down to the smallest size they can be.

## Adding Space To Columns

There are technically two ways we can add space to columns, one way though  might not be fully supported yet. 

The first one is: `gap`. If you set this property it will create a a gap of that size between the columns.  This is becoming more  widely supported though looking [here](https://caniuse.com/flexbox-gap).

The next thing you can do is sort of a trick and it is to use a combinator. You can do this like: `.col + .col`. 

What this is doing, is that it looks to see if the element has an adjacent sibling before it of that selector. If so, then it can select it. It's important to note that it only looks before it. You can then do a `margin-left` so you can create the space between the elements that you need to have a space between them.