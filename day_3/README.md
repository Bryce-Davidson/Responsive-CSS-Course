# Day 3 - Enter `max-width`

On this day Kevin begins talking about the max-width property.

max-width allows you to set a size for an element such that the element will not grow beyond that width upon being introduced on a larger screen sizes.

Kevin recomends using `max-width` with a pixel value.

## Challenge #2

For challenge #2 Kevin has us managing a content stretching issue where the body content is being stretched past the point of readability. Our goal is to be able to prevent the main body of the content from stretching to far as well as allowing the hero image background color to stretch from one side of the screen to the other.

## Solution

The solution I took was to break up the hero section of the document into it's own container with a class of hero and then since both the hero text content as well as the body content needed to be constrained to use the max-width we learned about, I wrapped both the text contents in a single div container with a class of margin.