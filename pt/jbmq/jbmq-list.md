# List Queues

>**Descrição**:
> Lista as filas de um ambiente.

- **Url Base**: `http://18.228.44.24:3000`
- **Path**: `/api/jbmq`
- **Method**: `GET`
- **Headers**

| Chave | Valor | Descrição |
|-------|-------|-----------|
| token | {{ token }} | Token gerado em [Harmony Login](../token/harmony-login.md) |

- **Parameters**

| Chave | Valor | Descrição |
|-------|-------|-----------|
| orgId | {{ orgId }} | Id da Organização em que deseja aplicar |
| envId | {{ envId }} | Id do ambiente em que deseja aplicar |

- **Curl**

```javascript
curl --location --globoff 'http://18.228.44.24:3000/api/jbmq?orgId={{orgId}}&envId={{envId}}' \
--header 'token: {{token}}'
```