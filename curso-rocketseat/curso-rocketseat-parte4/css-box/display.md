# display: block vs display: inline

- Como as caixas se comportam em relação às outras caixas
- Comportamento externo das caixas

## Diferenças

- **block** 
    - Ocupa toda a linha, colocando o próximo elemento abaixo desse
    - width e height são respeitados
    - padding, margin, border irão funcionar normalmente.

- **inline**
    - Elemento ao lado do outro
    - width e height não funcionam
    - somente valores horizontais de margin, padding e border

### Exemplos

block: tag `p`, `div`, `section`, todos os headings, `h1, h2`
inline: `a, strong, span, em`

```html
<div>
    block
</div>
<span>inline</span>
```

```css
div {
    height: 100px;
} /* Vai empurrar 100px o span */

span {
    height: 100px;
} /* Como span é inline, não vai empurrar 100px */
```

```css
div {
    display: inline;
}

span {
    display: block;
}

/* Mudando os displays */
```
