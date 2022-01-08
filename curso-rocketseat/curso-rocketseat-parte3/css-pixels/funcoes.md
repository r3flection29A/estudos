# Funções

Em programação, funções são reconhecidas por causar um reaproveitamento de código. 

* rgb()
* hsl()
* url()
* calc()

```html
<div class="box"></div>
```

```css
body {
    height: 100vh;
    margin: 0;
}

.box {
    height: calc(100% - 40px);
    width: 100%;
}
```

## Explicando o calc

Suponha que, queremos uma imagem que cubra 100% da altura da tela, mas queremos também que ele de um espaço de, por exemplo, 40 pixels. Para isso, usamos o calc. (Usar o codepen.io é uma boa ferramenta para ver isso em prática).
