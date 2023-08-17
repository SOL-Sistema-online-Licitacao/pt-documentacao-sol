---
description: Parâmetros de API para registrar uma licitação.
---

# POST BID/REGISTER

## Método POST para registrar uma licitação

Método **POST** para registrar uma licitação utilizando o SOL

**Endereço SOL Produção:**&#x20;

Parâmetros de requisição **BODY** form-data:

```
{
    "bid_count" : "1",
    "description" : "dadad",
    "agreement" : ObjectId("648a2831a3a2940e28acbd78"),
    "classification" : "obras",
    "start_at" : "",
    "end_at" : "1",
    "days_to_tiebreaker" : "1",
    "days_to_delivery" : "1",
    "deleted" : false,
    "local_to_delivery" : "rua salvador leme",
    "bid_type" : "individualPrice",
    "modality" : "openClosed",
    "status" : "draft",
    "aditional_site" : "www.site.com",
    "add_allotment" : [
        ObjectId("64bb1328e415630918ea433b")
    ],
    "invited_suppliers" : [

    ],
    "state" : "Amapá",
    "city" : "Ferreira Gomes",
    "association" : ObjectId("648a22356bc36bea837f9fd6"),
    "additionalDocuments" : [

    ]
}
```

**Retorno 201:**

<figure><img src="../../.gitbook/assets/Screenshot_13.png" alt=""><figcaption></figcaption></figure>

