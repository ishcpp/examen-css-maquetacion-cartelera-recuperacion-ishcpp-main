[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/I7gYMRAS)
# Examen práctico de CSS (recuperación)

En este examen se evaluará la aplicación de estilos CSS sobre una estructura HTML ya proporcionada.

El archivo `index.html` contiene la estructura completa de una página web. El objetivo consiste en aplicar estilos utilizando una hoja de estilos externa.

No se permite modificar la estructura HTML salvo que se indique explícitamente.

## Restricciones

Durante el examen no está permitido:

- modificar la estructura del HTML
- añadir estilos en línea
- usar etiquetas `<style>`
- utilizar `!important`

Todos los estilos deben escribirse en la hoja de estilos externa.

## 0. Enlazar la hoja de estilos

El documento HTML no incluye actualmente la referencia a la hoja de estilos.

Añadir en la sección `<head>` una etiqueta `<link>` que conecte el documento con el archivo:

```test
css/styles.css
```

## 1. Reset básico

Completar el bloque correspondiente para aplicar un reset básico.

Debe eliminarse el margen y el relleno por defecto de todos los elementos. Además, se debe configurar el modelo de caja mediante `box-sizing` para que el `padding` y el `border` se incluyan dentro del tamaño total definido para los elementos.

## 2. Estilos generales del documento

Configurar el estilo general del sitio aplicando reglas al elemento `body`.

Se debe definir:

- una tipografía sans-serif para todo el documento
- un color de texto para la página
- un color de fondo suave para el sitio

## 3. Cabecera con navegación integrada

El bloque `.cabecera` contiene el logo y la barra de navegación en la misma fila.

La cabecera debe:

- tener un color de fondo oscuro o intenso
- mostrar el texto en color claro para que exista contraste
- incluir espacio interno mediante `padding`
- utilizar Flexbox para colocar el logo y la navegación en horizontal, separados a los extremos (uno a cada lado)
- alinear verticalmente ambos elementos en el centro

El bloque `.cabecera` debe actuar como contenedor flex, distribuyendo el `.logo` y la `.navegacion` a cada extremo.

El título `.logo` debe tener un tamaño de fuente mayor que el texto normal.

## 4. Enlaces de navegación

Aplicar estilos a la navegación.

Se debe:

- eliminar el estilo de lista en `.lista-navegacion`
- distribuir los elementos del menú horizontalmente utilizando Flexbox
- añadir separación entre los elementos del menú

Los enlaces deben:

- eliminar el subrayado
- mostrar el texto en color claro

Además, al pasar el ratón sobre los enlaces debe cambiar su color.

## 5. Portada

Aplicar estilos al bloque `.portada`, situado bajo la cabecera.

La portada debe:

- tener un color de fondo distinto al del resto del sitio
- centrar el texto
- incluir un espacio interno amplio mediante `padding`

El título `.portada-titulo` debe tener un tamaño de fuente mayor que el texto normal.

## 6. Cartelera

El bloque `.cartelera` agrupa todas las tarjetas de película.

Se debe:

- utilizar Flexbox para distribuir las tarjetas
- permitir que las tarjetas pasen a la línea siguiente cuando no quepan, mediante `flex-wrap`
- añadir separación entre las tarjetas mediante `gap`
- incluir espacio interno en el contenedor mediante `padding`

## 7. Tarjetas de película

Aplicar estilos a cada elemento `.pelicula`.

Cada tarjeta debe:

- tener fondo blanco
- incluir espacio interno
- tener borde visible
- mostrar esquinas redondeadas
- aplicar una sombra mediante `box-shadow`
- tener un ancho fijo inferior al ancho total del contenedor, de forma que varias tarjetas quepan en la misma fila
- establecer `position: relative` para servir de referencia al distintivo de estreno

El título `.titulo-pelicula` debe separarse del contenido inferior.

Los párrafos dentro de `.pelicula` deben tener una pequeña separación inferior.

## 8. Distintivo de estreno

El elemento `.destacado` aparece solo en una de las tarjetas y debe mostrarse como una insignia situada en la esquina superior derecha de su tarjeta.

Recuerda que esto solo funciona si la tarjeta padre tiene establecido `position: relative` (punto 7).

Se debe:

- posicionar el distintivo de forma absoluta respecto a la tarjeta (`position: absolute`)
- colocarlo en la esquina superior derecha mediante `top` y `right`
- aplicar un fondo de color y texto en color claro
- incluir un pequeño espacio interno
- mostrar esquinas redondeadas

## 9. Etiquetas de género

Aplicar estilos al elemento `.genero`.

La etiqueta debe:

- tener un tamaño de fuente pequeño utilizando una unidad relativa
- mostrar un fondo de color
- utilizar `display: inline-block`
- incluir espacio interno
- tener esquinas redondeadas

## 10. Pie de página

Aplicar estilos al bloque `.pie-pagina`.

El pie debe:

- centrar el texto
- tener un fondo oscuro
- mostrar el texto en color claro
- incluir espacio interno
- separarse del contenido superior
