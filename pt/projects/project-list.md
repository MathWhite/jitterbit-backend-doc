# List Projects

>**Descrição**:
> Lista todos os projetos de uma organização.

- **Url Base**: `http://18.228.44.24:3000`
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
curl --location 'http://18.228.44.24:3000/api/projects?orgId={{orgId}}' \
--header 'token: {{token}}
```