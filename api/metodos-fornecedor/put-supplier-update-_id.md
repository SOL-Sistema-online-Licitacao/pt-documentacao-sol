---
description: Parâmetros de API
---

# PUT /SUPPLIER/UPDATE/{\_id}

## Método PUT para atualizar o fornecedor

Método **PUT** para atualizar o fornecedor pelo id do mesmo.

**Endereço SOL Produção:**&#x20;

**Requisição**

Obrigatório o ID do fornecedor

Parâmetros de requisição **BODY:**

```
{
  "name": "string",
  "cpf": "string",
  "type": "pessoa_fisica",
  "address": {
    "zipCode": "string",
    "publicPlace": "string",
    "neighborhood": "string",
    "city": "string",
    "state": "string",
    "latitude": "string",
    "longitude": "string",
    "complement": "string",
    "referencePoint": "string",
    "number": "string"
  },
  "legal_representative": {
    "name": "string",
    "nationality": "string",
    "maritalStatus": "solteiro",
    "cpf": "string",
    "rg": "string",
    "document_origin": "string",
    "validityData": "2023-08-17T19:26:51.642Z",
    "address": {
      "zipCode": "string",
      "publicPlace": "string",
      "neighborhood": "string",
      "city": "string",
      "state": "string",
      "latitude": "string",
      "longitude": "string",
      "complement": "string",
      "referencePoint": "string",
      "number": "string"
    }
  },
  "group_id": [
    "string"
  ],
  "categoriesId": [
    "string"
  ]
}
```

**Retorno 200:**

<figure><img src="../../.gitbook/assets/Screenshot_5 (6).png" alt=""><figcaption></figcaption></figure>

