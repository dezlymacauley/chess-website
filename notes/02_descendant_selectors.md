# Use this for targetting nested elements

This will make every `h1` element that is inside an `h1` purple,
regardless of how deep it is nested.
```css
h1 span {
    color: purple;
}
```
This will make every `h1` element that is directly inside an `h1` purple.
Any spans that are nested deeper will not be affected.
```css
h1 > span {
    color: purple;
}
```
