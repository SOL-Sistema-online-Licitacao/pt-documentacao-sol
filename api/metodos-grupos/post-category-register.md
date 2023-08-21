---
description: Parâmetros de API para registrar uma licitação.
---

# POST /CATEGORY/REGISTER

## Método POST para registrar uma categoria

Método **POST** para registrar uma nova categoria utilizando o SOL

**Endereço SOL Produção:**&#x20;

Parâmetros de requisição **BODY**:

{% hint style="info" %}
Em "category\_name", você deve utilizar uma das seguindes opções:

* obras
* servicos
* bens
{% endhint %}

```
{
  "category_name": "string",
  "segment": "string"
}
```

**Retorno 201:**

<figure><img src="../../.gitbook/assets/Screenshot_8 (3).png" alt=""><figcaption></figcaption></figure>

