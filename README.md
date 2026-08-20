# reset-admin — Restablecer contraseña (administradores)

Frontend standalone para el flujo de reset de cuentas admin (`POST /api/admins/forgot-password`).

## Marca

- UI alineada con **Kinecat** (mismo diseño que `reset/`)
- Soporte: `kinecatkinesiologia@gmail.com`

## Desarrollo local

```bash
npm install
npm start
```

Abrí `http://localhost:3000/reset-password?token=...&id=...` (token válido del email).

## Variables (.env)

Ver `.env.example`:

- `REACT_APP_API_URL` — backend (`https://kinapp-api.vercel.app/`)
- `REACT_APP_SUPPORT_EMAIL` — `kinecatkinesiologia@gmail.com`

## Deploy

Producción: `https://reset-admin-pass.vercel.app/`

Configurar en Vercel las mismas variables y apuntar el proyecto a este directorio/repositorio.

En `kinapp_api`, el link del email usa `RESET_ADMIN_URL` (default: reset-admin-pass.vercel.app).
