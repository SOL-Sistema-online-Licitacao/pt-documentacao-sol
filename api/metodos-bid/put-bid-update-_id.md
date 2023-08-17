---
description: Parâmetros de API
---

# PUT BID/UPDATE/{\_id}

## Método PUT para atualizar a licitação

Método **PUT** para atualizar a licitação pelo id da mesma.

**Endereço SOL Produção:**&#x20;

**Requisição**

Obrigatório o ID da licitação

Parâmetros de requisição **BODY:**

```
{
  "description": "string",
  "agreementId": "string",
  "classification": "string",
  "start_at": "string",
  "end_at": "string",
  "days_to_delivery": "string",
  "days_to_tiebreaker": "string",
  "local_to_delivery": "string",
  "status": "awaiting",
  "aditional_site": "string",
  "add_allotment": [
    {
      "allotment_name": "string",
      "days_to_delivery": "string",
      "place_to_delivery": "string",
      "quantity": "string",
      "files": "string",
      "add_item": {
        "group": "string",
        "item": "string",
        "quantity": "string",
        "unitMeasure": "string",
        "specification": "string"
      },
      "proposals": {
        "total_value": "string",
        "deleted": false,
        "status": "aguardando1",
        "item_list": [
          "string"
        ],
        "licitacaoId": "string",
        "proposedById": "string",
        "allotmentIds": [
          "string"
        ],
        "file": "string",
        "association_accept": false,
        "supplier_accept": false,
        "freight": 0
      },
      "status": "adjudicado"
    }
  ],
  "invited_suppliers": {}
}
```

**Retorno 201:**

<figure><img src="../../.gitbook/assets/Screenshot_13.png" alt=""><figcaption></figcaption></figure>

