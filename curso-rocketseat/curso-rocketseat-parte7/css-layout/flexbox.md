# Flexbox

* Nos permite posicionar elementos dentro da caixa
* Controle em uma dimensão (horizontal ou vertical)
* Alinhamento, direcionamento, ordernar e tamanhos

```css
div.parent {
    display: flex;
}
```

## flex-direction 

* Qual a direção do flex: horizontal ou vertical
* row | column 

## alinhamento

* justify-content
* align-items

```html
<div class="container">
    <div class="box blue"></div>
    <div class="box red"></div>
    <div class="box green"></div>
</div>
```

```css
.container {
    display: flex;
}
/* display flex vai fazer uma caixa ficar ao lado da outra */

/* para voltar ao padrão (block) usar o flex-direction: column */

/* justify-content: space-between => espaço responsivo entre os elementos */

/* justify-content: center => junta os elementos ao centro */

.box {
    width: 50px;
    height: 50px;
}

.blue {
    background-color: blue;
}

.red {
    background-color: red;
}

.green {
    background-color: green;
}
```

```css

body {
    margin: 0;
    height: 100vh;
    display: flex;
    align-items: center;
}
/* Vai alinhar os elementos ao centro */

.container {
    width: 100vw;
    display: flex;
    justify-content: center;
}
```

