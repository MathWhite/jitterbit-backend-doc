# Harmony Login Token (Apenas token)

>**Descrição**:
> Realiza o login na plataforma [Jitterbit Integration Studio](https://docs.jitterbit.com/integration-studio/) e retorna um `token` para ser utilizado nas demais API's, porém retorna apenas o token ao invés da lista de organizações do usuario. 

- **Url Base**: `http://18.228.44.24:3000`
- **Path**: `/api/login/token`
- **Method**: `POST`
- **Headers**

| Chave | Valor | Descrição |
|-------|-------|-----------|
| Content-Type | application/json | -- |

- **Body**

```javascript
{
    "login": "seu.email@jitterbit.com",
    "password": "sua_senha123"
}

``` 

- **Curl**

```javascript
curl --location 'http://18.228.44.24:3000/api/login' \
--header 'Content-Type: application/json' \
--data-raw '{
    "login": "seu.email@jitterbit.com",
    "password": "sua_senha123"
}'
```