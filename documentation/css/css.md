# CSS selectors

## Syntax
```css
selector {
    option: value;
}
```

Comment:
```css
/* This is a comment */
```

## Selectors
### Class
```css
.class-name {
    
}
```
### ID
```css
#id-name {
    
}
```

### Element
```css
h1 {

}
```

#### Element inside an element
```css
div h1 {
    /* This mean "any h1 inside a div" */
}
```

#### Multiple selections
```css
h1, p, div h2, h4, ... {
    /* This mean "h1 or p or ..." */
}
```

#### Direct child
```css
div > h1 {
    /* This mean "h1 direct inside a div" */
}
```

### Special selectors
```css
div:hover {
    /* apply style when you hover on it */
}
```

### Variables
```css
:root {
    --my-color: rgb(50, 80, 90);
    --base-padding: 50px;
    /* 
    You can set variables to use them in other 
    elements. 
    Name always needs to start with "--"
    */
}

div {
    background: var(--my-color);
    padding: var(--base-padding);
}
```