---
sidebar_position: 9
---
# 🔵 Lighthouse

Lighthouse es una herramienta de auditoría integrada en Chrome DevTools que analiza páginas web en cinco categorías clave para mejorar su calidad. Genera informes con métricas, puntuaciones y recomendaciones específicas.

![captura ejemplo](.\img\cap15.png)

## ¿Qué es Lighthouse?

Es una herramienta de código abierto creada por Google que:

- Evalúa el rendimiento, accesibilidad, SEO y buenas prácticas de una web.

- Proporciona puntuaciones (0-100) y sugerencias de mejora.

- Ayuda a optimizar la experiencia del usuario (UX) y el posicionamiento.

## Configuración del Informe Lighthouse

## Modo de Análisis
Define cómo se realiza la auditoría:

**Navigation (Default):**
Analiza la carga completa de la página (como un usuario que la visita por primera vez).

Útil para: Evaluar la carga inicial, renderizado y recursos críticos.

**Timespan:**
Mide interacciones durante un período específico (ej: clics, scroll).

Útil para: Analizar acciones del usuario después de la carga inicial.

**Snapshot:**
Captura el estado actual de la página (sin recargar).

Útil para: Auditar páginas con contenido dinámico (ej: SPAs).

## Dispositivo (Device)
Simula el entorno de prueba:

**Mobile:**
Emula un dispositivo móvil (red 4G, CPU limitada).

**Enfoque:**
 Rendimiento en móviles (Core Web Vitals, carga en 3G/4G).

**Desktop:**
Prueba en condiciones de escritorio (red rápida, mayor potencia).

**Enfoque:**
 Experiencia en navegadores de escritorio.

 ## Categorías a Evaluar

Selecciona qué aspectos auditar:

**Performance**	

- Mide Velocidad y optimización de carga.	

**Accessibility**	

- Mide Accesibilidad para usuarios con discapacidades.	

**Best Practices**

Cumplimiento de estándares web modernos.

**SEO**	

- Mide Optimización para motores de búsqueda.