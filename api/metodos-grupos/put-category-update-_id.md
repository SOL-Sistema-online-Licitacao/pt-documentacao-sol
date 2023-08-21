---
description: Parâmetros de API
---

# PUT /CATEGORY/UPDATE/{\_id}

## Método PUT para atualizar a categoria

Método **PUT** para atualizar a categoria pelo id da mesma.

**Endereço SOL Produção:**&#x20;

**Requisição**

Obrigatório o ID da categoria

Parâmetros de requisição **BODY:**

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

**Retorno 200:**

<figure><img src="../../.gitbook/assets/Screenshot_5 (5).png" alt=""><figcaption></figcaption></figure>

