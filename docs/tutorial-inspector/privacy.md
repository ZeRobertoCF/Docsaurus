---
sidebar_position: 8
---
# 🔵 Privacidad y seguridad



## Controles de Cookies de Terceros (Third-Party Cookies)

![captura ejemplo](.\img\cap17.png)


**¿Para qué sirve?**
- Simula el bloqueo de cookies de terceros (política actual de Chrome) para:

- Identificar funcionalidades rotas (ej: logins externos, widgets)

- Preparar tu sitio para la eliminación total de cookies de terceros

**Opciones clave:**

**🔒 Temporarily limit third-party cookies**

Activa restricciones solo cuando DevTools está abierto (modo prueba).

**🛡️ Excepciones (solo para casos especiales):**

**Third-party cookie grace period**

Permite cookies durante un período de transición (requiere registro oficial).

**Heuristics based exception**

Permite cookies automáticamente en escenarios como:

- Pop-ups de login

- Redirecciones OAuth (ej: "Iniciar sesión con Google")

- Flujos de pago embebidos


## Controls


![captura ejemplo](.\img\cap16.png)

Los Controls en Chrome DevTools son herramientas fundamentales para probar cómo se comportará tu sitio web bajo restricciones modernas de privacidad, específicamente con el bloqueo de cookies de terceros. Aquí te explico cada componente:

**1. Temporarily limit third-party cookies (Limitar temporalmente cookies de terceros)**

**Función principal:**

Simula el bloqueo de cookies de terceros solo mientras DevTools está abierto, permitiéndote:

- Identificar funcionalidades que dependen de estas cookies.

- Preparar tu sitio para el futuro sin cookies de terceros (planificado por Chrome).


**2. Exceptions (Excepciones)**

Escenarios especiales donde Chrome permite temporalmente cookies de terceros:

**A. Third-party cookie grace period (Período de gracia)**

**Para qué sirve:**

- Permite cookies de terceros durante un tiempo limitado si tu sitio está registrado en el programa de gracia de Chrome.

**Casos de uso:**

- Migraciones progresivas de sistemas legacy.

- Sitios con dependencias complejas en cookies externas.

**B. Heuristics based exception (Excepciones heurísticas)**

**Funcionamiento:**

Chrome detecta automáticamente situaciones donde las cookies son críticas y las permite temporalmente en:

- Pop-ups de login (ej: ventanas OAuth de Google).

- Redirecciones (flujos de autenticación cruzada).

- Iframes embebidos con interacción directa.

**3. Integración con el Panel de Privacidad**

Los Controls trabajan junto con otras secciones:

- Privacy > Third-party cookies: Muestra qué cookies se bloquean/permite.

- Security > Main origin: Verifica si el origen principal cumple con HTTPS y políticas CSP.

