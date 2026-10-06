# Use this for targetting nested elements

This will make every `h1` element that is inside an `h1` purple,
regardless of how deep it is nested.
```css
h1 span {
    color: red;
}

h1 span {
    color: purple;
}
```
This will make every `h1` element that is directly inside an `h1` purple.
Any spans that are nested deeper will not be affected.
```css
h1 span {
    color: red;
}

h1 > span {
    color: purple;
}
```
_______________________________________________________________________________

## Nesting

Another way to write a rule like this, is to use nesting.
```css
h1 span {
    color: red;
}

h1 span {
    color: purple;
}
```

This means any span nested inside the h1
```css
h1 {
    color: red;

    span {
        color: purple;
    }
}
```

This means any span directly nested inside the h1
```css
h1 {
    color: red;

    > span {
        color: purple;
    }
}
```
_______________________________________________________________________________
