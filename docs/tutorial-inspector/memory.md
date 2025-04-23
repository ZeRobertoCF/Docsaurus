---
sidebar_position: 7
---

# 🔵Memoria

Esta interfaz es una herramienta de perfilado de memoria en navegadores (probablemente Chrome DevTools) que ayuda a analizar el uso de memoria en aplicaciones web. A continuación explico cada sección:

## Tipos de perfilado de memoria


![captura ejemplo](.\img\cap11.png)

**Heap snapshot**
Captura una instantánea de la distribución de memoria en un momento específico.

- Uso: Muestra todos los objetos JavaScript y nodos DOM en memoria, permitiendo identificar qué ocupa más espacio.

**Allocations on timeline**
Registra asignaciones de memoria a lo largo del tiempo.

- Uso: Ayuda a detectar fugas de memoria al mostrar qué asignaciones persisten cuando no deberían.

**Allocation stack traces**
Registra los traces de pila para cada asignación de memoria.

- Nota: Genera más sobrecarga de rendimiento.

**Allocation sampling**
Aproxima las asignaciones de memoria mediante muestreo.

- Ventaja: Menor impacto en el rendimiento que otros métodos.

- Uso: Proporciona un desglose por pila de ejecución JavaScript.

**Detached elements**
Identifica elementos DOM que ya no están en el documento pero que aún son referenciados por JavaScript.

- Uso: Detecta fugas de memoria comunes donde elementos eliminados del DOM siguen ocupando memoria.

## Selección de instancia VM JavaScript

![captura ejemplo](.\img\cap12.png)

Muestra diferentes procesos/contextos de JavaScript con su consumo de memoria:

Columnas: Muestra el tamaño de memoria usado, la tasa de transferencia y la URL/origen.

Ejemplos:

- play.google.com usando 6.2 MB

- Un iframe de www.googleiagnanbager.com usando 20.1 MB

- Varios service workers (sw.js) con diferentes consumos

- webworksr.js usando 10.9 MB con alta tasa de transferencia (1198 KB/s)

## Resumen total

![captura ejemplo](.\img\cap13.png)

- Total JS heap size: 106 MB (tamaño total del montón JavaScript)

- Tasa de transferencia: 1198 KB/s (velocidad a la que se están moviendo datos)

## Botones de acción

![captura ejemplo](.\img\cap14.png)

[Load profile]: Para cargar un perfil de memoria guardado previamente.

[Take snapshot]: Para capturar una nueva instantánea del estado actual de la memoria.

Esta herramienta es esencial para optimizar aplicaciones web, identificar fugas de memoria y entender cómo se utiliza la memoria en tiempo real.