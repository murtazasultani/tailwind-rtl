# Tailwind rtl2
Tailwind CSS plugin to generate rtl variants.

## Installation

```bash
npm install tailwind-rtl2 --save-dev
```

## usage
```js
plugins: [
    require('tailwind-rtl2'),
    // ...
],
```

## Note
By default the `rtl` variant is not enabled to none of the tailwindcss utilities.
To use the `rtl` variant add it at the end of any utility you want to use it with.
You can toggle using the class `direction-rtl` at the parent element of your component

```js
variants: {
  alignContent: ['rtl'],
  alignItems: ['rtl'],
  alignSelf: ['rtl'],
  flex: ['rtl'],
  flexDirection: ['rtl'],
  flexGrow: ['rtl'],
  flexShrink: ['rtl'],
  flexWrap: ['rtl'],
  float: ['rtl'],
  inset: ['rtl'],
  justifyContent: ['rtl'],
  justifyItems: ['rtl'],
  justifySelf: ['rtl'],
  textAlign: ['rtl'],
  position: ['rtl'],
  margin: ['rtl'],
  translate: ['rtl'],
  rotate: ['rtl'],
  space: ['rtl'],
  borderWidth: ['rtl'],
  padding: ['rtl'],
  letterSpacing: ['rtl'],
  // ...
},
```

This plugin generates the following utilities:

```css
.direction-rtl {
  direction: rtl;
}

.direction-rtl .rtl\:flex-row {
  flex-direction: row;
}

.direction-rtl .rtl\:flex-row-reverse {
  flex-direction: row-reverse;
}
...
```
## Example

```html
<div class="mr-5 rtl:ml-5 rtl:mr-0">
    
</div>
```