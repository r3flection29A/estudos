# A cascata

A escolha do browser de qual regra aplicar, caso haja muitas regras para o mesmo elemento.

* Seu estilo é lido de cima para baixo

* É levado em consideração 3 fatores

1. Origem do estilo
2. Especificidade
3. Importância

### Origem do estilo

inline > tag style > tag link

```html
<h1 style="color: red;">Titulo</h1> <!-- mais importante -->

<style>
    h1 {
        color: red;
    }
</style> <!-- média importância -->

<link rel="stylesheet" href="style.css"> <!-- menos importante -->
```

### Especificidade

É um cálculo matemático onde cada tipo de seletor tem um valor.

0. Universal selector, combinators e negation pseudo-class (:not()) (0)
1. Element type selector e pseudo-elements (::before, ::after) (1)
2. Classes e attribute selectors ([type="radio"]) (10)
3. ID selector (100)
4. Inline (1000)

### !important

* quebra o fluxo natural da cascata
* serve para dar importância a um elemento

```html
<h1 class="title" id="my-title">Titulo <strong>teste</strong></h1>
```

```css
#mytitle, 
#mytitle, strong {
    color: gray;
}

.title {
    color: red;
}

h1 {
    color: blue !important;
} /* mesmo sendo o com menor valor, vai ter a maior importância com o !important */
```

