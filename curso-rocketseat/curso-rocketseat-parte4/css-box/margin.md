# Margin

Espaço entre os elementos 

- margin-top | margin-right | margin-bottom | margin-left
- values: `length` | `percentage` | `auto`

```css
div {
    /* shorthand */

    margin: 12px 16px 10px 4px;
    margin: 12px 16px 0;
    margin: 8px 16px;
    margin: 8px;

    /* top, right, bottom, left */
}
```

**Cuidado com o o collapsing (top se junto ao bottom)**

* Por padrão, há 8 pixels de margin do body

## Margin collapssing

```html
<div>
    margin
</div>
<section>margin2<section>
```

```css
* {
    margin: 0;
} /* tira a margin padrão definida pelo navegador */

div, section {
    border: 1px solid red;
    width: 100px;
    height: 100px;
}

div {
    margin-bottom: 8px;
}

section {
    margin-bottom: 8px;
}

/* Nada vai acontecer, pois estão se juntando. */
```

*Porém, se usarmos o display: inline, elas vão se juntar (usar o codepen.io)*

```css
div, section {
    border: 1px solid red;
    width: 100px;
    height: 100px;
    display: inline;
    margin: 0 2px;
} /* Lembre-se! O display inline só consegue aceitar margens laterais */
```

## Auto 

```css
div {
    margin: 0 auto;
} 
/* O auto faz um cálculo das laterais e "centraliza" o objeto, mas não faz esse cálculo nas partes de cima e em baixo */
```

