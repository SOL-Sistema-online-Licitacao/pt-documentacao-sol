# PUT /WORKPLAN/UPDATE/{id}

## Método PUT para atualizar um plano de trabalho

Método **PUT** para atualizar um plano de trabalho através do ID do mesmo.

**Endereço SOL Produção:**&#x20;

**Requisição**

Obrigatório o ID do plano de trabalho.

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
