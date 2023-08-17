---
description: Parâmetros de API para registrar uma licitação.
---

# POST /SUPPLIER/REGISTER

## Método POST para registrar um produto

Método **POST** para registrar um novo fornecedor utilizando o SOL

**Endereço SOL Produção:**&#x20;

Parâmetros de requisição **BODY**:

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
    "validityData": "2023-08-17T19:11:27.024Z",
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

**Retorno 201:**

<figure><img src="../../.gitbook/assets/Screenshot_9 (3).png" alt=""><figcaption></figcaption></figure>

