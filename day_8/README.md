# Day 8 - Flexbox Basics

Today we are beggining our pursuit into more complicated layouts with flexbox!

Kevin says this part of the course isn't a complete overview of flexbox but more a way we can get up and running with flexbox very quickly.

We are also jumping into challenge 4 which has to do with flexbox.

## Flex Container

The display property of an element specifies the type of the element, specifically we can use a `display: flex;` to turn the element into a `flex container`.

A flex container is an element that contains `flex items`. By default, a flex container will fit all of it's flex items into a single row which means shrinking each flex item down to the size of it's smallest piece of content if ncessary to fit all flex-items in a single line.

## Flex Items

Flex items are any elements that are contained within a flex container, that is a container which has the property `display: flex;` set.

Flex items are automatically shrunken down to thier smallest piece of content in order for the flex container to display all of them along the same row.

If we do not want the flex container to shrink the flex items down to the smallest peice of content, we can set an ideal size on the flex item by using a percentage on the width property such as `width: 100%` or equivalent.

## Defaults

On default a `display: flex` container will display the `flex-item` using the property `flex-direction: row` this indicates that each flex item will be placed along a single row and have thier borders shrunken if necessary to fit all items along the same axis.

`flex-containers` take into account the `flex-items` natural width.

A `flex-container` does not prioritize evenly distributing space to it's children proportionally, if it can shrink one down further according to its natural width, it will.

A `flex-container` only distributes the remaining space evenly if it cannot fit all of it's children along the row after shrinking them down to their natural width.

The priority of the steps above are as follows:

> natural width:
>
> the width of a element from it's supplied width or it's content

1. Fit everything along row
    2. If Can't
    - Shrink `flex-items` down to natural width
    - Evenly distribute space to `flex-items` which do not fit at natural width.
        - Overflow if space is smaller than `flex-items` smallest content.


## Gap Property

The `gap: ...;` property is a special property for `flex-containers` in order to place some space between all `flex-items` which doesn't affect the outside spacing.

`Warning!!` Gap is not well supported instead use the CSS selector `.col + .col` which specifies a combinator selector that selects an adjacent sibling if it exists. That is the first instance of the class `col` will not be selected because it does not have another instance of `col` before it.