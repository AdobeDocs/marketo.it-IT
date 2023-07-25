---
unique-page-id: 1900585
description: Aggiungere sezioni modificabili ai modelli e-mail v1.0 - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere sezioni modificabili ai modelli e-mail v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 1%

---

# Aggiungere sezioni modificabili ai modelli e-mail v1.0 {#add-editable-sections-to-email-templates-v1.0}

Se stai creando un modello nell’Editor modelli e-mail v1.0, puoi rendere modificabile qualsiasi sezione inserendo un’opzione `<div>` intorno a esso.

>[!NOTE]
>
>**Esempio**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Regole:

1. Il HTML deve essere sempre valido.
1. La classe di **MarketEditable** deve essere incluso.
1. L’ID deve essere univoco in tale HTML.
1. L&#39;ID non contiene spazi.

>[!CAUTION]
>
>Impossibile nidificare le istruzioni mktEditable.

Per informazioni su come eseguire questa operazione in Editor modelli e-mail v2.0, vedi [sintassi del modello e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
