# Page Layouts

- Tables
- Floats e clear
- Frameworks e Grid Systems
- Flexbox 
- Grid

## Posicionamentos

Controlar onde, na página, o elemento irá ficar, alterando o fluxo normal dos elementos.

- Name: position
- Value: static|relative|absolute|fixed

```html
<div class="box1 box"><div>
<div class="box2 box"></div>
<div class="box3 box"></div>
```

```css
.box {
    width: 50px;
    height: 50px;
    margin-bottom: 8px;
}

.box1 {
    background-color: red;
}

.box2 {
    background-color: green;
}

.box3 {
    background-color: aqua;
}
```

- Padrão => position: static 

## Relative 

- top, right, bottom, left, z-index

```css
.box1 {
    background-color: red;
    position: relative;
    left: 100px;
}
```

## Absolute

- top, right, bottom, left, z-index

- Absoluto em relação a página.

- Usar o codepen.io

## Fixed

```css
.box1 {
    position: fixed;
}
/* box1 fica fixo na página */
```

## Element Stacking

```css
.box1 {
    background-color: red;
    position: absolute;
    top: 5px;
    left: 5px;
    z-index: 3;
}

.box2 {
    background-color: green;
    position: absolute;
    top: 10px;
    left: 10px;
    z-index: 4;
}

.box3 {
    background-color: aqua;
    position: absolute;
    top: 15px;
    left: 15px;
    z-index: 4;
}

/* Surge uma nova linha (a z) que é o posicionamento de camadas. */
```




