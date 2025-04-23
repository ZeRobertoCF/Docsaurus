---
sidebar_position: 6 
---

# 🔵 Rendimiento

El panel Rendimiento en las herramientas de desarrollo del navegador es una herramienta avanzada para analizar el rendimiento de una página web, incluyendo métricas de carga, ejecución de JavaScript, renderizado y más.

## ¿Qué son las "Local Metrics"?

Son indicadores de rendimiento que miden la experiencia del usuario en tiempo real desde tu navegador, utilizando herramientas como Chrome DevTools o Lighthouse. Se enfocan en tres aspectos clave (Core Web Vitals de Google):

## Largest Contentful Paint (LCP) 

![captura ejemplo](.\img\cap7.png)

**Qué mide:**

El tiempo que tarda en cargarse el elemento más grande visible en la pantalla (por ejemplo: una imagen, un título o un bloque de texto).

**Objetivo ideal:**

- Bueno: ≤ 2.5 segundos (como en tu caso: 2.00 s ✅).

- Necesita mejora: Entre 2.5 y 4 s.

- Pobre: > 4 s.

## Interaction to Next Paint (INP) 

![captura ejemplo](.\img\cap10.png)

**Qué mide:**
El tiempo que tarda la página en responder a interacciones del usuario (clics, toques, teclas). Mide la latencia entre la acción y la actualización visual.

**Objetivo ideal**

- Bueno: ≤ 200 ms (tu valor: 104 ms ✅).

- Necesita mejora: Entre 200 y 500 ms.

- Pobre: > 500 ms.


## Cumulative Layout Shift (CLS) 

![captura ejemplo](.\img\cap8.png)

**Qué mide**
La inestabilidad visual acumulada (cuánto "salta" el contenido al cargarse). Se calcula basado en cambios inesperados en la posición de elementos.

**Objetivo ideal**

- Bueno: ≤ 0.1 (tu valor: 0.00 ✅).

- Necesita mejora: Entre 0.1 y 0.25.

- Pobre: > 0.25.
