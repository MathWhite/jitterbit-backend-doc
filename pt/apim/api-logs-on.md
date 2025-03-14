# Turn logs On

>**Descrição**:
> Liga o log de todas as API's de um [Environment](https://docs.jitterbit.com/management-console/environments/) por 7 dias.

- **Url Base**: `http://18.228.44.24:3000`
- **Path**: `/api/turnlogson`
- **Method**: `POST`
- **Headers**

| Chave | Valor | Descrição |
|-------|-------|-----------|
| Content-Type | application/json | -- |
| token | {{ token }} | Token gerado em [Harmony Login](../token/harmony-login.md) |

- **Parameters**

| Chave | Valor | Descrição |
|-------|-------|-----------|
| orgId | {{ orgId }} | Id da Organização em que deseja aplicar |
| envId | {{ envId }} | Id do ambiente em que deseja aplicar |


- **Curl**

```javascript
curl --location --request POST 'http://18.228.44.24:3000/api/turnlogson?orgId={{orgId}}&envId={{envId}}' \
--header 'Content-Type: application/json' \
--header 'token: {{token}}'
```