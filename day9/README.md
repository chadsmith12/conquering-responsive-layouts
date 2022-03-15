# Deeper Dive Into Flex Box

## Reducing Amount of HTML Needed

One thing that you can do to help you reduce markup is to move the class you were using onto the container `div` and have it be a `flex row` also. So where we were doing something like:

```html
<div class="container">
    <div class="row">
        ...
    </div>
</div>
```

You could combine it to be the following:

```html
<div class="container row">
    ...
</div>
```

With this approach one thing people start doing is creating "helper classes" to make something flex, vs. just caling it `row`. A commong approach is having a class called `d-flex` to signify `display: flex`.  Both approaches are fine and valid, it's just important to stick to one approach. Though make the `container` class flex might not be the best approach because there could be times you don't want the container to be `display: flex`.

## Column Wids and Flex Box

When you have a flex row it is common to want to have certain space between each column. By default each column will want to take up as much as it can. So if you two columns, they are both going to take up as much as they each could and it would be equal. There are times that maybe you want one one column to take up 60%  of the space. A common thing to do is to set `justify-content`.

By default `justify-content` will be set to `flex-start`. That will put the empty space on the trailing side. If you do `flex-end`, that will put the empty space on the leading side. If you do `center` then it will center the content and leave equal space on each side. The common value to set is: `space-between`. This will set all the space between the two items. So it would put the items to the leading and trailing respective.

