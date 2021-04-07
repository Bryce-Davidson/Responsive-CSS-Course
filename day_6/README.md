# Day 6 - Why you shouldn't use `em`s for font-size

Today kevin is teaching us some reasons it may not be the best idea to use ems for font sizes.

Kevin goes over some of the previous video content again in order to drive home the concept that because ems are a relative unit that get their measurment from the parent element you can get some pretty horrible cascading behaviour from them if you set them on certain elements such as a `<ul>` element;

![cascading-em](./cascading-em.png)