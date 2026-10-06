Applies to all elements with the `class="accent-text"`
```css
.accent-text {
    color: red;
}
```

Applies to all elements with the `class="bold-text"`
```css
.bold-text {
    font-weight: bold;
}
```

Applies to all elements with `class="accent-text bold-text"` (both classes)
```css
.accent-text.bold-text {
    text-decoration: underline;
}
```
_______________________________________________________________________________

## Using nesting

You can use nesting to write a rule like this...
```css
h2 {
  text-transform: uppercase;
}

h2.article-title {
  color: #973712;
}
```

...like this
```css
h2 {
  text-transform: uppercase;

    &.article-title {
        color: #973712; 
    }
}
```

The `&` is shorthand for the parent `h2`
_______________________________________________________________________________
