# List Project Details

>**Descrição**:
> Lista todos os projetos de uma organização junto com as informações de workflow, operations, crons e chunks configurados em cada projeto.

- **Url Base**: `http://18.228.44.24:3000`
- **Path**: `/api/projects/details`
- **Method**: `GET`
- **Headers**

| Chave | Valor | Descrição |
|-------|-------|-----------|
| Content-Type | application-json | -- |
| token | {{ token }} | Token gerado em [Harmony Login](/pt/token/harmony-login-token-only.md) |

- **Parameters**

| Chave | Valor | Descrição |
|-------|-------|-----------|
| orgId | {{ orgId }} | Id da Organização em que deseja aplicar |

- **Body**
> Para criar um relatório de crons, crie uma planilha no google drive, de acesso a `jitterbit-reporter@matheus-api-report.iam.gserviceaccount.com` e passe o id da planilha no campo `report.sheet_id`.

```javascript
{
    "params": {
        "only_schedules": false //para trazer apenas os schedules
    },
    "report": {
        "create_report": false, //para criar um relatório dos schedules (ambas flags em true)
        "sheet_id": "" //necessário planilha criada
    }
}
```

- **Curl**

```javascript
curl --location --request GET 'http://18.228.44.24:3000/api/projects/details?orgId={{orgId}}' \
--header 'token: {{token}}' \
--header 'Content-Type: application/json' \
--data '{
    "params": {
        "only_schedules": false
    },
    "report": {
        "create_report": false,
        "sheet_id": ""
    }
}'
```