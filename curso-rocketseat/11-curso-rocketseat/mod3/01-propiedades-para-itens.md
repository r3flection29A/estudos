# Propiedades para os itens

- flex-basis
- flex-grow
- flex-shrik
- flex
- order

## flex-basis

```css
.box {
  display: flex;
  border: 1px dashed red;
  gap: 100px;
}

.box div {
  border: 1px solid; 
  flex-basis: auto;
}

.box div:nth-child(1) {
  width: 25px;
}
```

## flex-grow

- O crescimento do item dentro do container em relação aos espaços vazios

```css
.box {
  display: flex;
  border: 1px dashed red;
}

.box div {
  border: 1px solid;
}

.box div:nth-child(3) {
  flex-grow: 1;
}
/* vai ocupar todo o espaço branco */
```

## flex-shrink 

- O item encolher dentro do container

```css
.box {
  display: flex;
  border: 1px dashed red;
  width: 160px;
}

.box div {
  border: 1px solid;
  flex-basis: 100%;
}

.box div:nth-child(2) {
  flex-shrink: 2;
}
/* vai encolher */
```

## flex

- shorthand 
- flex-grow flex-shrink flex-basis
- podem ter 1, 2 ou 3 valores

## Alterando o tamanho de múltipos itens

```html
<div class="page">
  <aside>Aside</aside>
  <main>
    Main
    <section>Content 1</section>
    <section>Content 2</section>
    <section>Content 3</section>
  </main>
</div>
```

```css
* {
  margin: 0;
  padding: 0;
  border-sizing: border-box;
}

.page {
  border: 2px solid;
  min-height: 100vh;
  display: flex;
}

aside {
  background-color: blue;
  flex: 1;
}

main {
  background-color: green;
  flex: 2;
  display: flex;
  flex-direction: column;
}

main section:nth-child(1) {
  background-color: grey;
  flex: 2;
}

main section:nth-child(2) {
  background-color: pink;
  flex: 1;
}

main section:nth-child(3) {
  background-color: red;
  flex: 1;
}
```

## order

```css
.box {
  display: flex;
  border: 1px dashed red;
}

.box div {
  border: 1px solid;
}

.box div:nth-child(1) {
  order: 1;
}

.box div:nth-child(2) {
  order: 0;
}

.box div:nth-child(3) {
  order: 0;
}

.box div:nth-child(4) {
  order: 0;
}
```
