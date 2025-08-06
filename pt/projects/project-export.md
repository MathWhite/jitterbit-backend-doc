# List Projects

>**Descrição**:
> Exporta para download um .ZIP com todos os projetos presentes em um ambiente.

- **Url Base**: `https://api.bakebell.cloud`
- **Path**: `/api/projects/exports`
- **Method**: `GET`
- **Headers**

| Chave | Valor | Descrição |
|-------|-------|-----------|
| token | {{ token }} | Token gerado em [Harmony Login](/pt/token/harmony-login-token-only.md) |

- **Parameters**

| Chave | Valor | Descrição |
|-------|-------|-----------|
| orgId | {{ orgId }} | Id da Organização em que deseja aplicar |
| envId | {{ envId }} | Id do ambiente em que deseja aplicar |

- **Curl**

```javascript
curl --location 'https://api.bakebell.cloud/api/projects/export?orgId={{ordId}}&envId={{envId}}' \
--header 'token: {{token}}
```