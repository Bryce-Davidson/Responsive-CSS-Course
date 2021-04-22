# Day 9 - Challenge 4 Solution, More Flexbox

Kevin goes on to explain that there are multiple ways here to structure our HTML so that we can reuse class functionality throughout the markup as well we can composite classes to simplify writing the markup.

## Flexbox Heights

Kevin gives an exmaple of how `flex-containers` work by altering the height of each of the `flex-items` to match eachother in order to align them in a row.

The dominant height is the height all of the other elements align to and coresponds to the element with the largest natural height.

One of the ways Kevin explains how we can change the height altering behaviour is to use `align-items: flex-start` or better yet, wrap whatever element we are concerned with height in a `<div>` element such that the `<div>` element is stretched and not the element within it.

Another way we can fix the height warp problem is to individually assign `align-self` on each of the items within the `flex-container`.

## Justify-Content

Justify content is all about how the `flex-items` are distributed within a `flex-container` and can change how we treat the extra space betweene elements.

Kevin explains that we can assign the widths of each element we want according to a `percentage` and then justify the content to maneuver the empty space.

We can use the properties such as `justify-content: space-between` in order to assign all of the extra space between each element and make sure that the left element is all the way to the left and the right element is all the way to the right.