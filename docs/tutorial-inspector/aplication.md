---
sidebar_position: 8
---

# 🔵 Aplicacion

Esta interfaz muestra información sobre las capacidades de almacenamiento y servicios en segundo plano de una aplicación web. Es parte de Chrome DevTools y ayuda a depurar tecnologías modernas de desarrollo web.

## Sección Principal: Application

1. Manifest
Función: Muestra el archivo manifest.json de la PWA (Aplicación Web Progresiva).

Uso: Verifica información como nombre, iconos, tema de color y capacidades de instalación.

2. Service Workers
Función: Gestiona los workers en segundo plano que permiten funcionalidad offline.

Uso: Depurar registro, actualización y comportamiento de los service workers.

3. Storage
Función: Administra todos los tipos de almacenamiento del navegador.

Uso: Inspeccionar y modificar datos almacenados localmente.

## Sección de Storage (Almacenamiento)

1. Local Storage
Almacenamiento persistente clave-valor (permanece después de cerrar el navegador).

2. Session Storage
Almacenamiento temporal clave-valor (se borra al cerrar la pestaña).

3. IndexedDB
Base de datos NoSQL para almacenar grandes cantidades de datos estructurados.

4. Cookies
Pequeños datos almacenados por el sitio web, enviados en cada petición HTTP.

5. Private State Tokens
API para prevención de fraude sin tracking entre sitios.

6. Interest Groups
Parte de la Privacy Sandbox para anuncios sin cookies de terceros.

7. Shared Storage
Almacenamiento entre sitios para casos de uso específicos con privacidad.

8. Cache Storage
Almacena respuestas de red para funcionalidad offline (usado por Service Workers).

9. Storage Buckets
Contenedores aislados para almacenamiento con diferentes políticas.

## Sección de Background Services
Servicios que pueden ejecutarse sin que la página esté activa:

- Back/forward cache: Optimización para navegación rápida.

- Background fetch: Descargas en segundo plano.

- Background sync: Sincronización cuando hay conexión.

- Bounce tracking mitigations: Protección contra tracking.

- Notifications: Notificaciones push.

- Payment handler: API de pagos.

- Periodic background sync: Sincronización periódica.

- Speculative loads: Precarga de recursos.

- Push messaging: Mensajería push.

- Reporting API: Reportes de errores/seguridad.

## Mensaje sobre Shared Storage
"No shared storage events detected" indica que no se han detectado eventos en el almacenamiento compartido, que es un mecanismo para compartir datos entre sitios de forma privada.

Esta herramienta es esencial para:

- Depurar PWAs

- Analizar el almacenamiento local

- Verificar el comportamiento offline

- Gestionar datos persistentes

- Depurar APIs modernas de privacidad y anuncios