# CSS Cheatsheet

## Basic Selectors

```css
element { property: value; }
.class-name { property: value; }
#id-name { property: value; }
```

## Combinators

```css
.parent .child { property: value; }
.parent > .child { property: value; }
.element1 + .element2 { property: value; }
.element1 ~ .element2 { property: value; }
```

## Pseudo-classes and Pseudo-elements

```css
a:hover { property: value; }
p::first-letter { property: value; }
```

## Box Model

```css
.element { margin: top right bottom left; border: width style color; padding: top right bottom left; }
```

## Display and Positioning

```css
.element { display: block | inline | inline-block | flex | grid | none; }
.element { position: static | relative | absolute | fixed | sticky; top: value; right: value; bottom: value; left: value; }
```

## Flexbox Layout

```css
.container { display: flex; flex-direction: row | row-reverse | column | column-reverse; flex-wrap: nowrap | wrap | wrap-reverse; justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly; align-items: flex-start | flex-end | center | baseline | stretch; align-content: flex-start | flex-end | center | space-between | space-around | stretch; }
.item { flex-grow: number; flex-shrink: number; flex-basis: length | auto; align-self: auto | flex-start | flex-end | center | baseline | stretch; }
```

## Grid Layout

```css
.container { display: grid; grid-template-columns: track1 track2 ...; grid-template-rows: track1 track2 ...; grid-template-areas: "area1 area2 ..." "area3 area4 ..."; grid-gap: row-gap column-gap; }
.item { grid-column-start: number | area-name; grid-column-end: number | area-name; grid-row-start: number | area-name; grid-row-end: number | area-name; grid-area: area-name; }
```

## Media Queries

```css
@media screen and (min-width: 768px) { /* Styles for screens larger than 768px */ }
@media screen and (max-width: 767px) { /* Styles for screens smaller than 768px */ }
```

## Clearfix

```css
.clearfix::after { content: ""; display: table; clear: both; }
```

## Center an Element Horizontally

```css
.center-horizontal { margin-left: auto; margin-right: auto; }
```

## Center an Element Vertically

```css
.center-vertical { position: absolute; top: 50%; transform: translateY(-50%); }
```

## Center an Element Vertically and Horizontally

```css
.center-both { position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); }
```

## Aspect Ratio Box

```css
.aspect-ratio-box { position: relative; width: 100%; padding-bottom: 56.25%; /* 16:9 Aspect Ratio */ }
.aspect-ratio-box > * { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }
```

## Truncate Long Text with Ellipsis

```css
.truncate-text { white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }
```

## Responsive Typography

```css
html { font-size: calc(16px + (24 - 16) * (100vw - 400px) / (1200 - 400)); }
```

## Smooth Scrolling

```css
html { scroll-behavior: smooth; }
```

## Custom Scrollbar

```css
::-webkit-scrollbar { width: 10px; }
::-webkit-scrollbar-track { background: #f1f1f1; }
::-webkit-scrollbar-thumb { background: #888; }
::-webkit-scrollbar-thumb:hover { background: #555; }
```

## Mobile First Media Query

```css
@media (min-width: 768px) {
  /* CSS rules for screens larger than or equal to 768px */
}
```

## Desktop First Media Query

```css
@media (max-width: 767px) {
  /* CSS rules for screens smaller than or equal to 767px */
}
```

## Breakpoints Example

```css
/* Extra Small Devices */
@media (max-width: 575px) {
  /* CSS rules for screens smaller than or equal to 575px */
}

/* Small Devices */
@media (min-width: 576px) and (max-width: 767px) {
  /* CSS rules for screens between 576px and 767px */
}

/* Medium Devices */
@media (min-width: 768px) and (max-width: 991px) {
  /* CSS rules for screens between 768px and 991px */
}

/* Large Devices */
@media (min-width: 992px) and (max-width: 1199px) {
  /* CSS rules for screens between 992px and 1199px */
}

/* Extra Large Devices */
@media (min-width: 1200px) {
  /* CSS rules for screens larger than or equal to 1200px */
}
```

## Responsive Typography

```css
html { font-size: calc(16px + (24 - 16) * (100vw - 400px) / (1200 - 400)); }
```

## Responsive Images

```css
img { max-width: 100%; height: auto; }
```

## Responsive Videos

```css
.video-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; }
.video-container iframe,
.video-container object,
.video-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }
```
