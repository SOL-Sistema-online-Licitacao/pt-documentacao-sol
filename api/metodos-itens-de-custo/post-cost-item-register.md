---
description: Parâmetros de API para registrar uma licitação.
---

# POST /COST-ITEM/REGISTER

## Método POST para registrar uma item de custo

Método **POST** para registrar um novo item de custo utilizando o SOL

**Endereço SOL Produção:**&#x20;

Parâmetros de requisição **BODY**:

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

**Retorno 201:**

<figure><img src="../../.gitbook/assets/Screenshot_8 (2).png" alt=""><figcaption></figcaption></figure>

