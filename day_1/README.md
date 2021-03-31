# Day 1 Challenge
## Don't Use Pixel-Width or Pixel-Height

### Summary

In this challenge Kevin required us to fix a nested container issue in which the child container of the parent container contained text which was overflowing the child container due to the height being set.

### Part 1 Solution:

To solve the child container text overflow problem I removed the pixel height attribute specified on the parent element to allow the parent container to flex with the window hwight, this is because Kevin had showed CSS is "naturally" responsive and "if the website is not responsive it is because we have set a constricting property to prevent this".

### Part 2 Solution:

To solve the second problem in which the child container was not responding to the parent containers resize as shown in the video I set the child containers width property to 50% to reflect the behaviour seen in the video. This allowed the child container to adapt to the parent container as the % values in CSS are set relative to the size of their parent containers.