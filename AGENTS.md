# Instrucciones para agentes de programación

## Objetivo
Este repositorio es una aplicación web estática de prueba para comprobar OpenCode, VS Code, GitHub Actions y GitHub Pages.

## Arquitectura
- `index.html`: interfaz accesible y responsive.
- `src/app.mjs`: interacción con la interfaz y almacenamiento local.
- `src/tasks.mjs`: lógica de negocio pura y comprobable.
- `src/style.css`: estilos.
- `test/`: pruebas automáticas con Node.js.
- `scripts/`: servidor de desarrollo y compilación.
- `docs/`: decisiones de arquitectura.

## Reglas
1. Responder y documentar en español.
2. Antes de modificar varios archivos, explicar el plan brevemente.
3. Mantener la separación entre lógica de negocio y acceso al DOM.
4. No añadir dependencias salvo necesidad justificada.
5. No introducir secretos en el repositorio o en el navegador.
6. No ejecutar `git push`, borrar archivos en masa ni publicar sin aprobación explícita.
7. Después de cambiar código, ejecutar `npm test` y `npm run build`.
8. Si algo falla, comunicar el error y no afirmar que las pruebas aprobaron.
9. Mantener accesibilidad básica: etiquetas, teclado, contraste y mensajes claros.
10. Toda nueva funcionalidad de lógica de negocio requiere una prueba.

## Comandos de verificación
- `npm run dev`: abrir aplicación en http://127.0.0.1:5173
- `npm test`: pruebas unitarias
- `npm run build`: genera `dist/` para despliegue
