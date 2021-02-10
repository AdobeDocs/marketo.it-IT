---
unique-page-id: 1900585
description: Aggiungere sezioni modificabili ai modelli e-mail v1.0 - Documenti Marketo - Documentazione prodotto
title: Aggiungere sezioni modificabili ai modelli e-mail v1.0
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# Aggiungere sezioni modificabili ai modelli e-mail v1.0 {#add-editable-sections-to-email-templates-v1.0}

Se state creando un modello nell&#39;Editor modelli e-mail v1.0, potete rendere modificabile qualsiasi sezione inserendo un `<div>` speciale attorno ad esso.

>[!NOTE]
>
>**Esempio**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Regole:

1. L&#39;HTML deve sempre essere valido.
1. È necessario includere la classe di **mktEditable**.
1. L’ID deve essere univoco in tale HTML.
1. Nessun spazio nell’ID.

>[!CAUTION]
>
>le istruzioni mktEditable non possono essere nidificate.

Per informazioni su come eseguire questa operazione in Editor modelli e-mail v2.0, controllare [sintassi modello e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
