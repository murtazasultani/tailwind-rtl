# Tailwind rtl
Tailwind CSS plugin to generate rtl variants.

## Installation

```bash
npm install tailwind-rtl
```

## usage
```js
plugins: [
    require('tailwind-rtl'),
    // ...
],
```

## Note
By default the `rtl` variant is not enabled to none of the tailwindcss utilities.
To use the `rtl` variant add it at the end of any utility you want to use it with.
You can toggle using the class `direction-rtl` at the parent element of your component

```js
variants: {
    alignContent: ['responsive', 'rtl'],
    alignItems: ['responsive', 'rtl'],
    alignSelf: ['responsive', 'rtl'],
    flex: ['responsive', 'rtl'],
    flexDirection: ['responsive', 'rtl'],
    flexGrow: ['responsive', 'rtl'],
    flexShrink: ['responsive', 'rtl'],
    flexWrap: ['responsive', 'rtl'],
    float: ['responsive', 'rtl'],
    inset: ['responsive', 'rtl'],
    justifyContent: ['responsive', 'rtl'],
    justifyItems: ['responsive', 'rtl'],
    justifySelf: ['responsive', 'rtl'],
    textAlign: ['responsive', 'rtl'],
    position: ['responsive', 'rtl']
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