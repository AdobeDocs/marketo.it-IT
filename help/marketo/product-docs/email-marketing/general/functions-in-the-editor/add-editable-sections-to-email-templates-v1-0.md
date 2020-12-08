---
unique-page-id: 1900585
description: Aggiungere sezioni modificabili ai modelli e-mail v1.0 - Documenti Marketo - Documentazione prodotto
title: Aggiungere sezioni modificabili ai modelli e-mail v1.0
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# Aggiungere sezioni modificabili ai modelli e-mail v1.0 {#add-editable-sections-to-email-templates-v1.0}

Se create un modello nell’editor modelli e-mail v1.0, potete rendere modificabile qualsiasi sezione inserendo un `<div>` elemento speciale attorno ad esso.

>[!NOTE]
>
>**Esempio**
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Regole:

1. L&#39;HTML deve sempre essere valido.
1. La classe di **mktEditable** deve essere inclusa.
1. L’ID deve essere univoco in tale HTML.
1. Nessun spazio nell’ID.

>[!CAUTION]
>
>le istruzioni mktEditable non possono essere nidificate.

Per informazioni su come eseguire questa operazione in Editor modelli e-mail v2.0, controllate la sintassi [del modello di](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)e-mail.
