---
unique-page-id: 1900585
description: Scopri come aggiungere sezioni modificabili ai modelli e-mail nella versione 1.0. Consenti agli utenti di modificare aree specifiche mantenendo il resto bloccato.
title: Aggiungere sezioni modificabili ai modelli e-mail v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
TQID: https://experienceleague.adobe.com/j2rwpy7Bq-HH3-mva5FkDb3kKH8cvlH2hMUp0ic7sno
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 111
ht-degree: 13%

---

# Aggiungere sezioni modificabili ai modelli e-mail v1.0 {#add-editable-sections-to-email-templates-v1.0}

Se stai creando un modello nell&#39;Editor modelli e-mail v1.0, puoi rendere modificabile qualsiasi sezione racchiudendola con uno speciale `<div>`.

>[!NOTE]
>
>**Esempio**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Regole:

1. Il HTML deve essere sempre valido.
1. La classe di **mktEditable** deve essere inclusa.
1. L’ID deve essere univoco in tale HTML.
1. L&#39;ID non contiene spazi.

>[!CAUTION]
>
>Impossibile nidificare le istruzioni mktEditable.

Per informazioni su come eseguire questa operazione in Email Template Editor v2.0, vedi [sintassi del modello e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
