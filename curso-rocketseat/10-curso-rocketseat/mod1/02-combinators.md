# Combinators 

Combinadores, pois eles trabalham para buscar e combinar seletores a fim de aplicar estilização.

## Descendant combinator

* Identificado por um espaço entre os elementos
* Busca um elemento dentro de outro

```css
body article h2

/* procure no body dentro de article o h2 */
```

## Child combinator

* Identificado pelo sinal `>` entre dois seletores
* Seleciona somente o elemento que é filho direto do pai
* Elementos depois do filho direto serão desconsiderados

```html
<body>
  <ul>
    <li>Item 1</li>
      <ul>
        <li>Item 2</li>
      </ul>
    </ul>
</body>
```

```css
body > ul > li {
    color: blue;
} 
/* vai colorir de azul apenas o filho direto */
```

## Adjacent sibling combinator

* Identificado pelo sinal `+` entre dois seletores
* Seleciona somente o elemento do lado direto que é irmão direto na hierarquia

```html
<h1>
  Titulo
</h1>

<p>
  Esse é um parágrafo 
</p>

<p>
  Outro parágrafo
</p>

<button>Um botao</button>
<button>Outro click</button>
```

```css
h1 + p {
    color: red;
}

button + button {
    margin-left: 32px;
}
```

## General sibling combinator

* Identificado pelo sinal `˜` entre dois seletores
* Seleciona todos os elementos irmãos


## Utilizado combinators
```html
<ul>
  <li>Aloo</li>
  <li class="red">Hey</li>
</ul>
```

```css
ul > li[class="red"] {
  color: red;
}
/* Vai pegar somente o li filho com a classe red */
```