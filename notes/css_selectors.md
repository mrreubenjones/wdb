# CSS Selectors

- Element
- Class
- ID
- Star
- Descendant
- Adjacent
- Attribute
- nth-of-type

### Element

Selects HTML elements directly. 

```css
a {
    color: #ffcccc;
}
```


### Class

Select elements by class names.

```css
.footnote {
    font-size: 1em;
}

```

### ID

Selects elements by id.

```css
#primary {
    border-top: 5px solid #ddd;
}

```


### Star

Selects all elements.

```css
* {
    background: #eee;
}
```


### Descendant

Selects elements based on hierarchy.

```css
.sidebar ul li a {
    text-decoration: none;
}
```


### Adjacent

Select elements that are positioned immediately after (adjacent) others. The following example would apply to all `p` tags that follow directly after an `h4`.

```css
h4 + p {
    margin-top: 1.2em;
}
```

### Attribute

Select elements with specific attributes.

```css
input[type="text"] {
    padding: 3px 2px;
}
```

### nth-of-type

Select "nth" element in a group.

```css
p:nth-of-type(1) {
    font-size: 1.4em;
}

.row:nth-of-type(even) {
    background: #f8f8f8;
}
```













