---
sidebar_position: 3
---

# 🔵 Consola

El panel Consola en las herramientas de desarrollo del navegador es una de las funciones más útiles para depurar, probar y entender el comportamiento de una página web. Aquí te explico detalladamente qué es, cómo usarla y ejemplos prácticos:

## Ver errores y advertencias
Si tu página tiene fallos, la consola los muestra:
```
javascript

undefinedFunction(); // ❌ Console: "Uncaught ReferenceError: undefinedFunction is not defined"
```
## Ejecutar código al instante
Puedes probar JavaScript sin modificar archivos:
```
javascript
// Calcular algo:
5 + 3; // ✅ Console: 8

//Modificar el DOM:

document.body.style.backgroundColor = "lightblue"; // Cambia el fondo de la página
```
## Depurar con console.log()
Imprime valores para entender el flujo del código:
```
javascript
let usuario = { nombre: "Ana", edad: 25 };
console.log("Datos usuario:", usuario); 
// ✅ Console: "Datos usuario: {nombre: 'Ana', edad: 25}"
```
## Interactuar con elementos HTML
Selecciona y manipula elementos:
```
javascript
// Cambiar texto de un botón:
document.querySelector("button").textContent = "¡Clic aquí!";


console.log(document.querySelectorAll("img")); // Lista las etiquetas <img>
``` 
## Probar API/fetch
Hacer solicitudes HTTP desde la consola:
```
javascript
fetch("https://jsonplaceholder.typicode.com/todos/1")
  .then(response => response.json())
  .then(data => console.log("Datos API:", data));
// ✅ Muestra los datos de la API en la consola
```
## Funciones avanzadas
- console.table(): Muestra datos en tabla:
```
javascript
let paises = [{ nombre: "México", capital: "CDMX" }, { nombre: "Argentina", capital: "Buenos Aires" }];
console.table(paises);
(Resultado: Tabla ordenada con columnas "nombre" y "capital").
```
- console.warn() / console.error():

```
javascript
console.warn("¡Atención! Esto es un aviso."); // Mensaje amarillo
console.error("Algo falló."); // Mensaje rojo
```
- Medir tiempo de ejecución:
```
javascript
console.time("test");
// Código a medir...
console.timeEnd("test"); // ✅ Muestra: "test: 0.25ms"
```