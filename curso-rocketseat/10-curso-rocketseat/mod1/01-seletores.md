# Seletores

Conecta um elemento HTML com o CSS a fim de alterar o elemento.

## Tipos

* Element selector
    - Todos os elementos HTML
* ID Selector
    - Um elemento que tenha o atributo `id`
    - Cada id deverá ser único
* Class Selector
    - Os elementos que contenha o atributo `class`
    - Podemos ter uma ou mais classes
* Attribute selector 
    - Um elemento que tenha um atributo específico
* Pseudo-class selector
    - Elementos em um estados específico

### Element selector
```html
<h1>Title</h1>
<p>Parágrafo</p>
```

```css
p {
    color: red;
}
```

### ID selector
```html
<h1 id="title">Title</h1>
<p id="content">Parágrafo</p>
```

```css
#content { 
    color: orange;
}
```

### Class selector
```html
<h1 id="title" class="red">Title</h1>
<p id="content" class="red">Parágrafo</p>
```

```css
.red {
    color: red;
}
```

### Attribute selector
```html
<h1 id="title" class="red" title="Algum título">Title</h1>
<p id="content" class="red">Parágrafo</p>
```

```css 
[title] {
    color: green;
}
```

### Pseudo-class selector
```html
<h1 id="title" class="red">Title</h1>
<p id="content" class="red">Parágrafo</p>
```

```css
h1:hover {
    color: green;
}
```

## Múltiplos

Você pode selecionar múltiplos elementos, com separação de vírgula, para selecionar múltipos elementos.

```css
h1, p, a {
    color: red;
}
```

