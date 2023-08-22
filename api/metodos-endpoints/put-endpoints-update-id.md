---
description: Parâmetros de API
---

# PUT /ENDPOINTS/UPDATE/{id}

## Método PUT para atualizar um endpoint

Método **PUT** para atualizar o endpoint pelo id do mesmo.

**Endereço SOL Produção:**&#x20;

**Requisição**

Obrigatório o ID do endpoint

Parâmetros de requisição **BODY:**

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

**Retorno 200:**

