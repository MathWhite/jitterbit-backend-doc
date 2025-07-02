# List Projects

>**Descrição**:
> Lista todos os projetos de uma organização.

- **Url Base**: `https://api.bakebell.cloud`
- **Path**: `/api/projects`
- **Method**: `GET`
- **Headers**

| Chave | Valor | Descrição |
|-------|-------|-----------|
| token | {{ token }} | Token gerado em [Harmony Login](/pt/token/harmony-login-token-only.md) |

- **Parameters**

| Chave | Valor | Descrição |
|-------|-------|-----------|
| orgId | {{ orgId }} | Id da Organização em que deseja aplicar |

- **Curl**

```javascript
curl --location 'https://api.bakebell.cloud/api/projects?orgId={{orgId}}' \
--header 'token: {{token}}
```