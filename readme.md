# CSS - Sesión 4.1

1. Es un lenguaje para dar estilos a la web (1996)


## SINTAXIS

- Como se puede establecer codigo CSS

```css
h1 {
    color: red;
}
```

- h1: selector
- color: propiedad
- red: valor

## CONCEPTOR IMPORTANTES DE CSS

- 4 conceptos importantes de CSS

### SELECTORES

- Indica a q elemento o elementos se aplicara los estilos

```css
h1 {
    /* selector de etiqueta */
    color: red;
}

/* selector de descendencia */
nav ul li a {
    color: red;
}

a {
    /* aplica a todo */
    color: red;
}
```

### HERENCIA

- Elementos ancestros (padre) heredan algunas propiedades a sus descendientes.

```html
    <p>Hola Mundo <a href="#">Esto es un enlace</a></p>
```

```css
p {
    color: green
}

a{
    color: inherit;
}
```

### CASCADA

- Significa que los estilos que llegan en ultimo lugar sobreeescriben a los anteriores.


```css
h1 {
    color: red
}

p {
    color: green
}

a{
    color: inherit;
}

h1 {
    color: blue
}
```

### ESPECIFICIDAD

- Es un valor numerico que adquieren los selectores y se aplica cuando hay conflictos.
- La especificidad vence a la cascada

```html
<!-- Selector de etiqueta (1) -->

<!-- Selector de clase (2) -->

<!-- Selector de ID (3) -->

<!-- INLINE (1000) --> 

<!-- IMPORTANT (infinito) -->
```

# ESTILO DE TEXTO

- fonts.google.com para descargar tipos de fuentes y tipografias
- font-face css (mdn)


## PROPIEDADES

- color
- font-size (em, rem, px)
- font-weight
- font-family (google font, font-face)
- estilo entre navegadores (normalize.css)
- text-transform: uppercase / lowercase / capitalize
- text-align: left / center / right
- letter-spacing: 
- word-spacing:
- text-decoration: none / underline

## SELECTORES

- selector de etiqueta
- selector de clase
- selector de ID
- selector universal (uso box model)

<!-- Actualizar el repositorio con lo visto en la 2da parte
  1) Explicar los conceptos con ejemplos
  2) (Agregar una nueva tipografia de google fonts, usando font-face)
-->