# Actualizaciones TsOrbit Coins

Manifest remoto servido en Cloudflare Pages:

`https://actualizacionescoinstsorbit.pages.dev/update.json`

## Publicar una update

1. Sube el APK a `public/downloads/tsorbit-coins.apk` (o cambia `downloadUrl`).
2. Edita `public/update.json`:
   - `latestVersion`: versión nueva (ej. `1.0.2`)
   - `minVersion`: mínimo obligatorio (si la app está por debajo → update forzada)
   - `force`: `true` para bloquear “Más tarde”
   - `enabled`: `false` para desactivar el modal
3. Commit + push a `main` (Actions despliega Pages).

La app compara contra su `APP_VERSION` en `src/appVersion.ts` / `app.json`.
