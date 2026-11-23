# Decisiones de arquitectura

## Objetivo
Validar un flujo OpenCode + VS Code + GitHub Actions + GitHub Pages sin base de datos, API de pago o framework.

## Componentes
- HTML y CSS: interfaz.
- Módulo `src/app.mjs`: interacción y almacenamiento local.
- Módulo `src/tasks.mjs`: lógica pura, probada con Node.js.
- Pruebas nativas `node --test`.
- Build con módulos nativos de Node; publicación únicamente de `dist/`.

## Límites conocidos
- Las tareas viven en `localStorage`, no se sincronizan entre dispositivos.
- No hay autenticación ni almacenamiento en servidor.
- GitHub Pages sirve únicamente archivos estáticos.

## Evolución
Cuando sea necesario, crear API, base de datos, autenticación y despliegue backend por separado.
