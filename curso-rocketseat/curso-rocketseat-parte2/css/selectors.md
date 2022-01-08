# Selectors

Conecta um elemento HTML com o CSS

## Tipos

* Global selector `*` => todos os elementos
* Element/type selector `h1, h2, p, div` => elementos
* ID Selector `#box, #container` => id 
* Class Selector `.red, .m-4` => classes
* Attribute selector, Pseudo-class, Pseudo-element, e outros

## Exemplo

```html
<body>
    <div class="container">
        <h1 id="title">Título</h1>
        <p>Lorem Ipsum</p>
    </div>
</body>
```
### Indo pro CSS

```css
* {
    background-color: gray;
    margin: 0;
    padding: 0;
}

.container {
    background: blue;
}

#title {
    font-size: 60px;
}

p {
    display: inline-block;
}
```

