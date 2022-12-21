---
unique-page-id: 1900585
description: Aggiungere sezioni modificabili ai modelli e-mail v1.0 - Documenti Marketo - Documentazione del prodotto
title: Aggiungere sezioni modificabili ai modelli e-mail v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 1%

---

# Aggiungere sezioni modificabili ai modelli e-mail v1.0 {#add-editable-sections-to-email-templates-v1.0}

Se crei un modello nell’Editor modelli e-mail v1.0, puoi rendere modificabile qualsiasi sezione inserendo uno speciale `<div>` intorno.

>[!NOTE]
>
>**Esempio**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Regole:

1. Il HTML deve essere sempre valido.
1. La classe di **mktEditable** deve essere incluso.
1. L&#39;ID deve essere univoco in quel HTML.
1. Nessun spazio nell&#39;ID.

>[!CAUTION]
>
>Impossibile nidificare le istruzioni mktEditable.

Per informazioni su come eseguire questa operazione in Editor modelli e-mail v2.0, consulta [sintassi del modello e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
