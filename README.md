# Actualizaciones TsOrbit Coins

Sitio: `https://actualizacionescoinstsorbit.pages.dev`

La app solo usa ese link. Al tocar **Actualizar ahora** abre esta página para descargar.

## Cómo publicar una update

1. Sube el APK (o el instalador) a `public/` (ej. `public/tsorbit-coins.apk`).
2. Edita `public/update.json` en este repo (versión, título, mensaje, `enabled: true`).
3. Push a `main` → se despliega en Pages.

Campos de `update.json` (todo remoto, nada en la app):

- `enabled` — si `false`, no muestra modal
- `latestVersion` — versión nueva
- `minVersion` — si la app está por debajo, fuerza update
- `force` — oculta “Más tarde”
- `title` / `message` / `changelog` — texto del modal
