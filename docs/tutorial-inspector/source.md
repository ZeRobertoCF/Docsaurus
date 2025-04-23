---
sidebar_position: 4
---

# 🔵 Fuentes

El panel "Sources" (o "Fuentes") en las herramientas de desarrollo del navegador es una de las secciones más potentes para desarrolladores. Se divide en tres partes principales, cada una con funciones específicas:

![captura ejemplo](.\img\cap3.png)

## Parte 1: Panel de Archivos (File Navigator)
**Qué es:** 
Un explorador de archivos que muestra todos los recursos cargados por la página web (HTML, CSS, JS, imágenes, etc.), organizados por origen (dominio, carpeta, etc.).

**Para qué sirve:** 

- Navegar por la estructura de archivos de la página.

- Buscar archivos específicos (usando Ctrl + P).

- Ver el código fuente original (incluso si está minificado, con opción "Pretty Print").

- Editar código temporalmente (los cambios se pierden al recargar).

**Ejemplo práctico:** 
Si quieres modificar el CSS de un botón:

- Busca el archivo .css en el panel.

- Haz clic para ver su contenido.

- Edita una propiedad (ej: color: red;).

Los cambios se aplican al instante en la página (solo en tu navegador).

## Parte 2: Editor de Código (Code Editor)
**Qué es:** 
Un editor integrado donde se visualiza y edita el código de los archivos seleccionados.

**Para qué sirve:** 

- Depurar código JavaScript con breakpoints.

- Modificar HTML/CSS/JS en vivo (sin afectar el código real).

- Trazar la ejecución línea por línea.

- Guardar cambios locales (en algunos navegadores como Chrome).

**Ejemplo práctico:** 
Para depurar un bucle:

- Abre el archivo .js en el editor.

- Haz clic en el número de línea para añadir un breakpoint.

- Recarga la página: la ejecución se pausará allí.

- Usa los controles de depuración (▶️, ⏸️) para avanzar paso a paso.

## Parte 3: Panel de Depuración (Debugging Tools)
**Qué es:** 
Un conjunto de herramientas para analizar el comportamiento del código (variables, call stack, breakpoints, etc.).

**Para qué sirve:**

- Inspeccionar variables en tiempo real (pestaña Scope).

- Ver la pila de llamadas (Call Stack).

- Gestionar breakpoints y condiciones.

- Monitorizar eventos del DOM (Event Listener Breakpoints).