---
sidebar_position: 5
---

# 🔵 Redes

El panel Network (Red) en las herramientas de desarrollo del navegador es una herramienta fundamental para monitorear y analizar todas las solicitudes HTTP/HTTPS que realiza una página web.

Registra en tiempo real todas las interacciones entre el navegador y los servidores, incluyendo:

- Solicitudes de archivos (HTML, CSS, JS, imágenes, fuentes, etc.).

- Llamadas a APIs (AJAX/fetch).

- WebSockets y otros recursos.

## Barra de controles superiores 

![captura ejemplo](.\img\cap4.png)


**Preserve log (Conservar registro):**
Mantiene las solicitudes visibles incluso al recargar la página. Útil para depurar flujos con redirecciones.
Ejemplo: Si envías un formulario y la página se recarga, activa esto para ver la solicitud POST.

**Disable cache (Desactivar caché):**
Fuerza al navegador a descargar todos los recursos desde el servidor, ignorando la caché local.
Ejemplo: Si modificas un archivo CSS pero no ves cambios al recargar, activa esta opción.

**No throttling (Sin limitación de red):**
Permite simular conexiones lentas (ej: 3G) para probar rendimiento en diferentes condiciones.
Ejemplo: Selecciona "Fast 3G" para ver cómo carga tu sitio en móviles con conexión limitada.

## Filtros
**Filtrar por tipo de recurso:**

Fetch/XHR: Llamadas a APIs (AJAX/fetch).

JS/CSS: Archivos JavaScript o hojas de estilo.

Img/Media: Imágenes o videos.
Ejemplo: Filtra por XHR para debuggear una API que no devuelve datos.

**Filtrar por tiempo:**
La barra de tiempo (ej: 50,000 ms) ayuda a identificar solicitudes lentas.
Ejemplo: Haz clic en 400,000 ms para ver qué recursos tardan más de 400ms.

**Invert (Invertir):**
Oculta los recursos que coinciden con el filtro.
Ejemplo: Filtra CSS y activa "Invert" para ocultar archivos CSS.


## Tabla de solicitudes 


![captura ejemplo](.\img\cap5.png)

Muestra detalles clave de cada solicitud:


![captura ejemplo](.\img\cap6.png)


**Análisis de tus datos:**

- Las solicitudes con Status: 204 (No Content) son comunes en llamadas a APIs que no devuelven datos (ej: tracking).

- La solicitud que tardó 1.55 s podría ser un cuello de botella (revisa su Timing).


## ¿Para qué sirve?

**Debuggear APIs:**

- Filtra por XHR > Busca errores (Status: 4xx/5xx) > Revisa Headers y Response.

**Optimizar imágenes:**

- Filtra por Img > Ordena por Size > Comprime imágenes pesadas.

**Analizar rendimiento:**

- Usa Throttling para simular 3G y detectar recursos lentos.

