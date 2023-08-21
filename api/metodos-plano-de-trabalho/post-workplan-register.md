# POST /WORKPLAN/REGISTER

## Método PUT para atualizar o status de um lote

Método **PUT** para atualizar o status de um lote através do ID do mesmo.

**Endereço SOL Produção:**&#x20;

**Requisição**

Obrigatório o ID do lote.

Parâmetros de requisição **BODY:**

```
{
  "name": "string",
  "product": [
    {
      "quantity": 0,
      "unitValue": 0,
      "costItems": "string"
    }
  ]
}
```

**Retorno 200:**
