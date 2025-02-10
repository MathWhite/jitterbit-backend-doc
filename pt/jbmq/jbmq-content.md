# List Queue Content

>**Descrição**:
> Lista os 1000 primeiros registros (e seus conteúdos) de uma fila.

- **Url Base**: `http://18.228.44.24:3000`
- **Path**: `/api/jbmq/content`
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
| queueName | {{ queueName }} | Nome da fila que deseja ler |

- **Curl**

```javascript
curl --location --globoff 'http://18.228.44.24:3000/api/jbmq/content?orgId={{orgId}}&envId={{envId}}&queueName={{queueName}}' \
--header 'token: {{token}}'
```