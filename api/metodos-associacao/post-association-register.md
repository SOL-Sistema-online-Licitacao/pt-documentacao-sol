---
description: Parâmetros de API para registrar uma licitação.
---

# POST /ASSOCIATION/REGISTER

## Método POST para registrar uma associação

Método **POST** para registrar uma nova associação utilizando o SOL

**Endereço SOL Produção:**&#x20;

Parâmetros de requisição **BODY**:

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
    "validityData": "2023-08-17T17:41:01.048Z",
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

**Retorno 201:**

<figure><img src="../../.gitbook/assets/Screenshot_12 (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

