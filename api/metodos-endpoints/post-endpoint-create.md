---
description: Parâmetros de API para registrar uma licitação.
---

# POST /ENDPOINT/CREATE

## Método POST para criar um novo endpoint

Método **POST** para criar um novo endpoint utilizando o SOL

**Endereço SOL Produção:**&#x20;

Parâmetros de requisição **BODY**:

```
{
  "endpointPath": "string",
  "token": "string",
  "frequency": "string",
  "lastRun": null,
  "status": "stopped",
  "endpointType": "association"
}
```

**Retorno 201:**

