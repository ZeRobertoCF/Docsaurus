---
sidebar_position: 2
---
# 🔵 Elementos

El panel Elements (o Inspector de elementos) en las herramientas de desarrollo del navegador te permite ver y editar el código HTML y CSS de una página web en tiempo real. Es especialmente útil para analizar la estructura de un sitio, depurar problemas de diseño o experimentar con cambios antes de implementarlos en el código real.

## ¿Para qué sirve el panel Elements?

## Inspeccionar la estructura HTML

Ver la jerarquía de etiquetas (DOM) de la página.

Ejemplo: Si pasas el cursor sobre un ```<div> ``` en el inspector, el navegador resalta ese elemento en la página.

![captura ejemplo](.\img\cap1.png)

## Editar HTML y CSS al instante

Puedes modificar texto, atributos (class, id), o incluso eliminar nodos HTML para probar cambios.

Ejemplo: Cambiar temporalmente el texto de un botón de "Enviar" a "Clic aquí".

```html

<button class="btn">Enviar</button>

<button class="btn">Clic aquí</button>
```

## Ajustar estilos CSS

Ver y editar reglas de CSS aplicadas a cualquier elemento.

Ejemplo: Cambiar el color de un botón desde el panel Styles:

```css
.btn {
  background-color: blue; /* Original */
  background-color: red;  /* Modificado en el inspector */
}
```
![captura ejemplo](.\img\cap2.png)

## Analizar el modelo de caja (Box Model)

Visualizar márgenes (margin), rellenos (padding), bordes (border) y dimensiones de un elemento.

Box Model en Chrome
(Imagen: Desglose del Box Model de un elemento)

## Depurar diseño responsivo

Identificar por qué un elemento no se adapta bien en móviles (ej.: un width fijo en píxeles).