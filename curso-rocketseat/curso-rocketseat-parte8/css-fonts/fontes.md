# Fontes

Tipografia transmite mensagem 

    - negrito
    - tamanho
    - estilo

## Basic Font Properties

* font-family
* font-weight 
* font-style
* font-size

## Font family

* Tipo de fonte de um elemento 
* Lista de fontes e ordem de prioridade
* inclui *falback* font

```css
p {
    font-family: "Times New Roman", Times, serif;
}
/* se o navegador não tiver a Times New Roman, ele vai pular pra Times e assim ocorre para o serif. */
```

## Font Weight

* Peso da fonte

```css
p {
    font-weight: bold;
}
/* Dependendo da família da fonte, não tem todos os pesos */

/* Os pesos são => normal | bold | lighter| 100 ... 900 */
```

## Font style 

* É o estilo da fonte 
* Valores => normal | italic | oblique
* Os valores que podem ser aplicados dependem da fonte

```css
span {
    font-style: italic;
}
```

## Font size

* Tamanho da fonte

```css
p {
    font-size: 30px;
}
```

## Web fonts

- Fontes do sistema x Fontes da web
- como usar fontes para web? 

    * @font-face
    * @import 
    * link

## Font variant

* Faz variações na apresentação da fonte 

```css 
p {
    font-variant: small-caps;
}
```
https://developer.mozilla.org/en-US/docs/Web/CSS/font-variant

## Font stretch

* alargamento ou encolhimento da fonte
* aceita palavras-chaves como: expanded, condensed, normal
* aceitar porcentagens de 50% a 200%

```css
p {
    font-stretch: expanded;
}
```
https://developer.mozilla.org/en-US/docs/Web/CSS/font-stretch

## Letter spacing 

* Espaçamento entre as letras 

```css
p {
    letter-spacing: 1px;
}
```

## Word spacing

* Espaçamento entre as palavras

```css
p {
    word-spacing: 3px;
}
```

## Line height

* Espaço entre linhas

```css 
p {
    line-height: 1.6;
}
```

## Text transform 

* Mudança de texto

* Valores => none | capitalize | uppercase | lowercase | full-width | full-size-kana

```css 
p {
    text-transform: uppercase;
}
```

## Text decoration 

* Aparência decorativa de um texto 
* line => underline, overline, line-through
* style => wavy, dotted, double, dashed, solid
* color => `color` values

```css
p {
    text-decoration: underline solid red; /* shorthand */
}
```

## Text align 

* Alinhamento de texto 

```css
p { 
    text-align: center;

    /* pode ser right, left ou justify */
}
```

## Text shadow

* Sombra no texto

```css
p {
    text-shadow: 1px 1px 1px 1px red;
}
```

