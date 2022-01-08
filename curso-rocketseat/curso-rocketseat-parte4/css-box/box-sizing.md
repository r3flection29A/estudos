# box-sizing 

Como será calculado o tamanho total da caixa? 

content-box|border-box

```css
div {
    box-sizing: border-box;
}
```

```css
div {
    width: 100px;
    height: 100px;
    border: 1px solid red;
    margin: 10%;
    padding: 0 20px;
}
/* Vai aumentar para 140 pixels de largura. Usar o codepen.io para melhor visualização */
```

### Como fazer que continue como 100px e não somar o padding? 

Com o border-box! 

```css
div {
    width: 100px;
    height: 100px;
    border: 1px solid red;
    margin: 10%;
    padding: 0 20px;
    box-sizing: border-box;
}
/* Manterá os 100 pixels de largura e o padding de 20 pixels, não irá somar */
```
