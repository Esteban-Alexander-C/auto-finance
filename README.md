# AutoFinance

Aplicación web de finanzas personales con registro automático de pagos desde Android y métricas configurables.

> **Nota:** AutoFinance es una aplicación **web** (accesible desde cualquier navegador, también en el móvil). Android solo interviene en la captura automática de pagos, mediante una automatización ya existente en el teléfono, sin app nativa propia.

## Objetivo del proyecto

Reducir al mínimo el esfuerzo de llevar el control del dinero. La mayoría de apps de gastos se abandonan porque obligan a registrar cada pago a mano. AutoFinance permite registrar cada gasto en segundos, con captura automática desde el móvil Android, y lo convierte en un historial claro y en métricas útiles (como el gasto hormiga), ajustables a los criterios de cada usuario.

## Tecnologías que se van a utilizar

| Capa | Tecnología |
|---|---|
| Frontend (panel web) | Angular (TypeScript) |
| Frontend (registro rápido móvil) | React |
| Backend (API REST) | ASP.NET Core (C#) con autenticación mediante tokens |
| Base de datos | SQL Server + Entity Framework |
| Despliegue | Azure (App Service, Azure Functions) o AWS |
| Captura de pagos | Automatización en Android (MacroDroid / Tasker / HTTP Shortcuts) |
| Opcional | Power Automate como conector adicional |

## Alcance inicial

- API REST con autenticación y endpoint para registrar gastos (`POST /gastos`).
- Registro manual de gastos desde el panel web (base que siempre funciona).
- Base de datos con gastos y ajustes de usuario.
- Panel web en Angular con:
  - Historial de gastos (importe, comercio, fecha, individual/pareja).
  - Total por periodo.
  - Gasto hormiga, con umbral configurable por el usuario.
- Fases posteriores: automatización de captura en Android, despliegue en la nube, métricas avanzadas (suscripciones, comparativas) y vista de registro rápido en React.

## Autor

**Esteban Alexander Laica Caizaguano** — [@Esteban-Alexander-C](https://github.com/Esteban-Alexander-C)
