# Transiciones CSS

Las transiciones en CSS nos permiten aplicar un cambio de estilo gradual a los elementos del documento HTML. Además, nos ofrecen la ventaja de poder especificar el tiempo para que se produzca la transformación entre estilos, de esta forma podríamos utilizarlas para dar un efecto de animación.

Todos los parámetros para aplicar las transiciones se pueden establecer en una sola línea y también mediante propiedades por separado. Veamos cómo se implementa en una sola línea.

**Formato:**

```css
transition: [propiedad a modificar] [Duración] [Tipo de animación] [Retardo];
```

**Ejemplo:**

```css
.caja1 {
    background-color: #c0392b;
    transition: background-color 1s linear;
}
.caja1:hover {
    background-color: #3f51b5;
}
```

## Significado de las propiedades:

### [Propiedades a modificar]

Algunas de las propiedades que podemos modificar utilizando transiciones son las que se muestran en la siguiente lista:

```
all
background-color
border
border-radius
color
top
bottom
left
right
box-shadow
width
height
line-height
margin
opacity
word-spacing
letter-spacing
fill
padding
stroke
text-shadow
vertical-align
visibility
z-index
```

### [Duración]

Es necesario especificar la cantidad de tiempo y la unidad de medida que va a durar la animación.

Por ejemplo: `3s 👉 (3 segundos).` `250ms 👉 (250 milisegundos)`

### [Tipo de animación]

Esta propiedad es opcional y sirve para indicar la velocidad de la animación. Algunas de las posibilidades son las siguientes:

-   **linear**: la velocidad de la animación es uniforme en todo el recorrido.
-   **ease**: la velocidad se acelera al inicio, luego se retarda un poco y se acelera al final de nuevo.
-   **ease-in**: la animación empieza lentamente y va aumentando progresivamente.
-   **ease-out**: la animación empieza muy rápida y va descendiendo progresivamente.
-   **ease-in-out**: la animación empieza y acaba lentamente, y es en la parte central del recorrido donde la velocidad es más rápida.

### [Retardo]

Tiempo (en segundos o milisegundos) que el navegador esperará antes de poner en marcha la animación.

Por ejemplo: `1s 👉 (1 segundo).`
