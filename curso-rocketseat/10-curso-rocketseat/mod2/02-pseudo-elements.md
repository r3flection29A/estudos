# Pseudo-elements

Como pseudo-elements podemos adicionar elementos HTML pelo próprio CSS

`::pseudo-element-name`

## Exemplos

* ::befor
* ::after
* ::first-line

```html
<li>A</li>
<li>A</li>
<li>A</li>
<li>A<li>
```

```css
li::after {
    content: ">"
}

li::before {
    content: "_"
}

p::first-line {
    font-weight: bold;
}