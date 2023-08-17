---
description: Parâmetros de API
---

# PUT /COST-ITEM/UPDATE/{\_id}

## Método PUT para atualizar o item de custo

Método **PUT** para atualizar o itemde custo pelo id do mesmo.

**Endereço SOL Produção:**&#x20;

**Requisição**

Obrigatório o ID do item

Parâmetros de requisição **BODY:**

```
{
  "code": "string",
  "name": "string",
  "unitMeasure": "M",
  "categoryId": "string",
  "productId": "string",
  "specification": "string",
  "sustainable": true,
  "product_relation": "string"
}
```

**Retorno 200:**

<figure><img src="../../.gitbook/assets/Screenshot_5 (3).png" alt=""><figcaption></figcaption></figure>

