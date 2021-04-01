# Day 2 Notes

In todays lesson we are learning about the relative units _rem_ and _em_.

Kevin begins the lesson by providing [this youtube video](https://www.youtube.com/watch?v=_-aDOAMmDHI) as a introduction and comprehensive tutorial on _em_ and _rem_.

## Relative Units

### em

In the world of web design em has to do with *font-sizes*.

`1em = 16px`

If you set a font-size using em it will be in relation to that elements parent font-size.

That is, if the parent element has a font-size `n` then a child element with a font-size of `xem` will have a font-size of `x * n`.

for _ems_ the compounding of font-sizes is *active*, that is if there are multiple generations of elements inside a parent element the last child element will have a compound font-size relative to the parent element made up of all it's predecessors.

### rem

What _rem_ stands for is _root em_ which is a reference to the `<html>` element's font-size.

for _rems_ compounding of font-sizes is _inactive_.

### em with any other property

_em_ has a slightly different behaviour with margin & padding and any other property where instead of looking at the parent element's margin & padding it looks at the current elements font-size.

#### Example

```css
.parent {
 font-size: 3em;
}

.child {
    // looks at .parent font-size
    font-size: 2em;         2 * 3 = 6

    // looks at .child font-size
    margin-bottom: 2em;     6 * 2 = 12
}
```

The same kind of behaviour does not apply to _rem_, because _rem_ is always looking at the `<html>` element.

### Why This is Helpful?

The fact that properties other than the font-size such as margin and padding look at the *elements font-size* is extremely useful when adjusting the font-size of a element as these other properties set in _em_ ensure that all we have to focus on is the elements font-size and the container will adjust to the text.

### Where can you get caught up?

You can get caught up when setting the margin of a group of elements _em_ but then any element that inherits that class with a different font-size will have the margin set relative to its font-size.

## Summary

`em` (font-size) -> parent font-size

`em` (not font-size) -> element font-size

`rem` (any property) -> `<html>` font-size



## Do's and Don'ts

### Why you shouldn't set font-sizes using em

Compounding font-sizes is a common problem in CSS so it's often better to set font-sizes with `rem` and then set all other properties relative to this font-size using `em`.

