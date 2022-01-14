# Pseudo-classes

É um tipo de seletor que irá selecionar um elemento que estiver num estado específico.

EXEMPLO: É o primeiro elemento dentro de uma caixa, ou, o elemento está com o ponteiro do mouse em cima dele.

Pseudo-classes começam com 2 pontos seguido do nome da pseudo-class `:pseudo-class-name`

## Selecionando elementos com pseudo-classes

* :first-child
* :nth-of-type()
* :nth-child()

```html
<ul>
    <li>Gratidão</li>
    <li>Esperança</li>
    <li>Fé</li>
</ul>
```

```css
ul li:first-child {
    font-weight: bold;
}
/*  pega o primeiro filho no caso o primeiro li */
```
```html
<article>
    <h3>Gratidão</h3>
    <p>Lorem...</p>
    <p>Lorem</p>
    <p>Lorem</p>
</article>
```

```css
article p:nth-of-type(1) {
    font-weight: bold;
}
/* vai pegar o primeiro elememento do tipo p */
```

```css
article p:nth-child(1) {
    font-weight: bold;
}
/* PEGA OS CHILDS, no caso, o h3 */
```

### odd e even
```html
<ul>
    <li>Gratidão</li>
    <li>Esperança</li>
    <li>Fé</li>
    <li>Gratidão</li>
    <li>Esperança</li>
    <li>Fé</li>
</ul>
```

```css 
ul li:nth-child(even) {
    background-color: red;
} 
/* números pares */
```
```css
ul li:nth-child(odd) {
    background-color: grey;
}
/* números ímpares */
```

## Ações do usuário

* :hover
* :focus

```html
<a href="#">Clique aqui</a>
<input type="text">
```

```css
a:hover {
    color: red;
}
/* Vai mostrar o link vermelho ao passar o mouse */
```

```css
input:focus {
    border-color: red;
}
/* Vai mostrar uma borda vermelha a focar no input */
```

## Atributos

* :disabled
* :required

```html
<input type="text" disabled>
<input id="1" type="password" required>
```

```css
input:disabled {
    background-color: grey;
}

#1:required {
    background-color: blue;
}
```


