# consent_admin

Admin dashboard (Next.js on port 3001 locally). Own Azure App Service.

## Local

```bash
pnpm install
cp .env.example .env
pnpm dev   # http://localhost:3001
```

Requires `consent_api` on port 4000.

## Azure

Node **22** Linux Web App. GitHub secret `AZUREAPPSERVICE_PUBLISHPROFILE`. Optional variables: `AZURE_ADMIN_APP`, `ADMIN_URL`, `WEB_URL`, `API_URL`.
