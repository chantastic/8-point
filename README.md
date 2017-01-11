# 8-point
A set of 8 point grid classes.

## Why

[8-point grid](https://spec.fm/specifics/8-pt-grid) is a thing.
It's a good thing at that.

8 has a lot of advantages as a number.
It's chief adavntage is that it bifurcates evenly.
So devices that do any type of strange scaling don't end up with half-values.

This is good.

This lib just offers a set of classes for using an 8-point soft grid with the css box model. It incluedes classes for `margin`, `padding`, `TRBL`, `width`, `height`, and "size".

## Anatomy

The class names break down like this:

```txt
{acronymized CSS property}-{n × 8px}
```

For example:

```css
.p-1 { padding:  8px }  /* 1 × 8px */
.p-2 { padding: 16px } /* 2 × 8px */
.p-3 { padding: 24px } /* 3 × 8px */
```

You can use side-specific properties as well:

```css
.mt-1 { margin-top: 8px }
.mr-1 { margin-right: 8px }
.mb-1 { margin-bottom: 8px }
.ml-1 { margin-left: 8px }

/* x and y added for convenience */

.my-1 { margin-top: 8px; margin-bottom: 8px }
.mx-1 { margin-right: 8px; margin-left: 8px }
```

## Legend

#### properties

```txt
m  = margin
mt = margin-top
mr = margin-right
mb = margin-bottom
ml = margin-left
my = margin-top; margin-bottom
mx = margin-right; margin-left

p  = padding
pt = padding-top
pr = padding-right
pb = padding-bottom
pl = padding-left
py = padding-top; padding-bottom
px = padding-right; margin-left

t = top
r = right
b = bottom
l = left

w = width
h = height

s = width; height
```

#### values

```txt
1 = 8px
2 = 16px
3 = 24px
4 = 32px
5 = 40px
6 = 48px
7 = 56px
8 = 64px
```

## Install
NPM:
`npm i -S 8-point`

## Use
```html
<div class="m-1 p-3">
  This has 8px margin and 24px padding.
</div>

<img
  src="./path/img.ext"
  class="s-8"
  alt="this img is 64px high and wide"
/>
```

## License

MIT License

Copyright (c) 2016 Michael Chan
