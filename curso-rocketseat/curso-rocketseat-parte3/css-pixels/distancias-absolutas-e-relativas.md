# Distâncias absolutas 

São fixas e não alteram seu valor. 

Exemplos: 
**cm, in, px**

* o mais comum é o **px**
* não recomendado usar o cm

# Distâncias relativas

São relativas a algum outro valor, pode ser o elemento pai, ou root, ou o tamanho da tela.

* Benefícia: Maior adaptação aos diferentes tipos de tela.

Exemplos: 
**em, rem, vw, vh**

* em => Tamanho da font do pai
* rem => Tamanho da font do elemento raiz (root/html)
* vw => 1% da viewport width
* vh => 1% da viewport height

```html
<div>
    <p>Parágrafo</p>
</div>
```

```css
div {
    font-size: 18px;
}
p {
    font-size: 1em;
}

/* Ou seja, o elemento filho (p) dobrou o tamanho da fonte de 18 pixels do elemento pai (div) */
```

E se eu quiser não pegar do elemento pai e sim do elemento root? (o padrão)

```css
div {
    font-size: 18px;
}

p { 
    font-size: 2rem;
}

/* Vai dobrar o padrão, que no caso do p é 16px */
```

E se quiser mudar o padrão?

```css
:root {
    font-size: 16px;
} /* ou html */
```

