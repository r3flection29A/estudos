# Propiedades do Flex Container 

* Direção dos itens
* Multi linhas
* Alinhamento
    * principal
    * cruzado
* espaço entre os itens

## Direção dos itens
- Flex é uma dimensão (horizontal ou vertical)
- podemos mudar a direção com `flex-direction`
- valores (row | row-reverse | column | column-reverse)

```html
<div class="container">
    <div class=item>A</div>
    <div class=item>B</div>
    <div class=item>C</div>
</div>
```

```css
.container {
  display: flex;
  flex-direction: column-reverse; /* reverte a coluna */
}
/* row é padrão */
/* row-reverse de trás para frente */
/* column muda o eixo principal e vira uma coluna */
```

## Flex-wrap

- Podemos usar multi linhas
- Cada nova linha, um novo flex container

```html
<div class="box">
  <div>A</div>
  <div>B</div>
  <div>C</div>
  <div>D</div>
</div>
```

```css
.box {
  display: flex;
  flex-wrap: wrap;
  border: 1px dashed red;
}

.box div {
  border: 1px solid;
  width: 80px;
}
```

## flex-flow

- shorthand
- flex-direction || flex-wrap

## justify-content 

- alinhamento dos elementos dentro do container 
- distribuição dos elementos

### valores

- flex-start
- flex-end 
- center
- space-around
- space-between
- space-evenly

## align-items

- alinhamento dos elementos no eixo cruzado

### valores

- stretch (padrão)
- flex-start
- flex-end
- center

## gap

- Espaço entre os elementos

### valores

- unidades de medida