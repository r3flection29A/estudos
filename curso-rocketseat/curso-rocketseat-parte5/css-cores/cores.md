# Cores 

Usamos o CSS para alterar as cores dos documentos.

## Tipos

* background-color (para caixas)
* color (para textos)
* border-color (para caixas)
* outros...

## Valores

Podemos definir os valores por

* palavra-chave (blue, transparent)
* hexadecimal (#990011)
* funções: `rgb`, `rgba`, `hsl`, `hsla`

```css
element {
    /* Keyword values */
    
    color: currentcolor;

    /* <named-color> values */
    
    color: red;

    /* <hex-color> values 0-F */
    
    color: #090; /* RED GREEN BLUE */
    color: #009900;
    color: #090a;
    color: #009900aa;

    /* rgb() */

    color: rgb(34, 12, 64, 0.6) /* 0-255 */

    /* hsl() */

    color: hsl(30, 100%, 50%, 0.6) /* Hue - Saturation - Lumiance */

    /* Global Values */

    color: inherit;
    color: initial; 
    color: unset;
}
