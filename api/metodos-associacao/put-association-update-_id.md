---
description: Parâmetros de API
---

# PUT /ASSOCIATION/UPDATE/{\_id}

## Método PUT para atualizar a associação

Método **PUT** para atualizar a associação pelo id da mesma.

**Endereço SOL Produção:**&#x20;

**Requisição**

Obrigatório o ID da licitação

Parâmetros de requisição **BODY:**

```
{
  "name": "string",
  "cnpj": "string",
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
  "legalRepresentative": {
    "name": "string",
    "nationality": "string",
    "maritalStatus": "solteiro",
    "cpf": "string",
    "rg": "string",
    "document_origin": "string",
    "validityData": "2023-08-17T17:53:18.455Z",
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
  }
}
```

**Retorno 200:**

<figure><img src="../../.gitbook/assets/Screenshot_5 (2) (1).png" alt=""><figcaption></figcaption></figure>

