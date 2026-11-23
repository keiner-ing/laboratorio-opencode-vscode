---
name: Revisión de calidad
description: Ejecuta una lista de verificación de pruebas, build, seguridad y documentación antes de proponer un commit
---

# Procedimiento de calidad

1. Lee `AGENTS.md` y `docs/architecture.md` desde la raíz del repositorio.
2. Identifica los archivos modificados y determina cuáles requieren pruebas.
3. Ejecuta `npm test` y registra el resultado real.
4. Ejecuta `npm run build` y comprueba que `dist/index.html` exista.
5. Comprueba accesibilidad básica, errores visibles y ausencia de secretos.
6. Resume resultados y pendientes. No hagas `git push` ni despliegues sin autorización.
