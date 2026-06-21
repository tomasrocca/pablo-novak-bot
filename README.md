# Pablo Akinator — Vercel

Bot web de Pablo Novak / Villa Epecuén listo para deploy en Vercel.

## Variables de entorno necesarias

En Vercel, agregar:

- `ANTHROPIC_API_KEY`: tu API key de Anthropic.
- `ANTHROPIC_MODEL`: opcional. Por defecto usa `claude-sonnet-4-6`.

## Probar local

```bash
npm install
npm i -g vercel
vercel login
vercel dev
```

Crear un archivo local `.env` si querés probarlo en tu compu:

```bash
ANTHROPIC_API_KEY=tu_api_key
ANTHROPIC_MODEL=claude-sonnet-4-6
```

## Subir a GitHub

```bash
git init
git add .
git commit -m "Deploy Pablo Akinator"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/pablo-akinator-vercel.git
git push -u origin main
```

## Deploy con Vercel

Opción simple:

1. Entrá a Vercel.
2. New Project.
3. Importá el repo de GitHub.
4. En Environment Variables agregá `ANTHROPIC_API_KEY`.
5. Deploy.

O por terminal:

```bash
vercel
vercel env add ANTHROPIC_API_KEY
vercel --prod
```
