# consent_admin

Independent admin UI in its own GitHub repo and Azure App Service (`consentadmin`). It only talks to **consent_api** over HTTPS (`NEXT_PUBLIC_API_URL`). It does not host or deploy the API.

Local API: `http://localhost:4000/api/v1`  
Azure API: `https://consentapi-abgrbph5cfccbxe0.eastus2-01.azurewebsites.net/api/v1`

## Local

```bash
pnpm install
cp .env.example .env
pnpm dev   # http://localhost:3001
```

## Azure

Node **22** Linux Web App `consentadmin`:
https://consentadmin-fwb7gmeybmhwhyd0.eastus2-01.azurewebsites.net

Calls API `https://consentapi-abgrbph5cfccbxe0.eastus2-01.azurewebsites.net/api/v1`. Secret `AZUREAPPSERVICE_PUBLISHPROFILE`. App name default `consentadmin`.
