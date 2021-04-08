# Day 8 - Flexbox Basics

Today we are beggining out pursuit into more complicated layouts with flexbox!

Kevin says this part of the course isn't a complete overview of flexbox but more a way we can get up and running with flexbox very quickly.

## Flex Container

The display property of an element specifies the type of the element, specifically we can use a `display: flex;` to turn the element into a `flex container`.

A flex container is an element that contains `flex items`. By default, a flex container will fit all of it's flex items into a single row which means shrinking each flex item down to the size of it's smallest piece of content if necessary.

## Flex Items

Flex items are any elements that are contained within a flex container, that is a container which has the property `display: flex;` set.

Flex items are automatically shrunken down to thier smallest piece of content if necessary in order for the flex container to display all of them along a row.

If we do not want the flex container to shrink the flex items down to the smallest peice of content, we can set an ideal size on the flex item by using a percentage on the width property such as `width: 100%`.