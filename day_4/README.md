# Day 4 - viewport-units

Today we learn about some more relative CSS units of measurment, the viewport-units.

The viewport can be thought of as the rectangular space which a device has available to display content. On a mobile device this is much smaller and on a desktop device is much larger. The inteded goal of the v-units is expose units of measrument relative to the actual viewing device.

The viewport units are very good for expressing content padding such that we have a padding that is relative to whichever device is viewing our content. Just as well, the viewport-units are good for expressing title font-sizes as this ensures that no matter which device is viewing our content we aren't getting text that is too small or too big.

When using viewport units for type, we can always express a specific size of type for really small screens and one for really big screens and have the viewport-units handle everything in between.

## vh

The `vh` unit is a representation of the **viewport height** which means we can *always* load a conent block at the full height, or half the height of the viewport of the viewing device.

## vw

Just the same as the `vh` unit, the `vw` unit is a representation of the **viewport width** which means we can have content displayed with a *relative size* to the actual viewing device.

### How do these differ from 100%?

Both `vh` and `vw` are relative units of measurement relative to the *viewing device* while 100% is always a relative unit to the *parent container*.

## vmax

`vmax` is a special case of both `vh` and `vw` where `vmax` will convert itself to whichever of `vh` or `vw` is bigger depending on the viewport.

## vmin

`vmin` does the exact same thing as `vmax` except it will convert itself