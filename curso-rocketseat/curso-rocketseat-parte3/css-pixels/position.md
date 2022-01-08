# Posições 

position

Representa um conjunto de coordenadas 2D: 
- top, right, bottom, left e center
* usado para alguns tipos de propiedades
* não confundir com a propiedade `position`

```html
<div class="box"></div>
```

```css
.box {
    width: 400px;
    height: 300px;
    background-image: url(http://image.com/random);
    background-repeat: no-repeat; /* padrão é repeat */
    background-position: right 50px;
    /* 50 pixels para a direita, assim vale para todas as posições. Right, top, bottom, left e center */
}
```

