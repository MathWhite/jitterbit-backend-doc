# List Queues

>**Descrição**:
> Lista as filas de um ambiente.

- **Url Base**: `https://api.bakebell.cloud`
- **Path**: `/api/jbmq`
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
curl --location --globoff 'https://api.bakebell.cloud/api/jbmq?orgId={{orgId}}&envId={{envId}}' \
--header 'token: {{token}}'
```