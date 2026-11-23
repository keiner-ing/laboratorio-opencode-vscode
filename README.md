# Laboratorio OpenCode + VS Code

Proyecto web estático con tareas persistidas en `localStorage`, pruebas, skill, agente especializado y pipeline CI/CD.

## Requisitos
Node.js LTS (recomendado 26), npm, Git, VS Code y OpenCode 2.

## Ejecutar
```bash
npm ci
npm test
npm run build
npm run dev
```
Abre http://127.0.0.1:5173 en el navegador. Detén con Ctrl+C.

## Integrar OpenCode
Desde esta carpeta, ejecuta `opencode`. Luego ejecuta `/connect` para conectar tu proveedor y `/models` para elegir el modelo.

Pruebas útiles para el agente:
- `Lee AGENTS.md y explica la arquitectura sin editar archivos.`
- `Usa la skill revision-calidad y verifica las pruebas y el build.`
- `Usa el subagente reviewer para revisar el código sin editarlo.`

## Publicar
1. Crear un repositorio en GitHub con rama `main`.
2. Subir código con Git o `gh repo create`.
3. En GitHub, abrir Settings > Pages y seleccionar **GitHub Actions**.
4. Hacer un push a `main`: se ejecutan pruebas, build y publicación.

La publicación de GitHub Pages es pública y no soporta backend; solo se sube `dist/`.

## Seguridad
No incluir `.env`, claves API, datos de clientes ni material privado en este repositorio.
