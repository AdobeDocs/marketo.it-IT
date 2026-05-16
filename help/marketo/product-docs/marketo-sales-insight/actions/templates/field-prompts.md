---
description: Scopri i prompt dei campi nei modelli e-mail. Aggiungi segnaposto che richiedono al mittente di compilare il contenuto personalizzato durante l’invio.
title: Prompt dei campi
exl-id: c138b627-f853-4d35-b022-cc517d6b86d4
TQID: https://experienceleague.adobe.com/ahVbX8SGxaVUjSPsU-1uVc36ecIW60lwYXxDZSxC0kU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 175
ht-degree: 2%

---

# Prompt dei campi {#field-prompts}

I prompt dei campi ti consentono di aggiungere una stringa di testo alle e-mail che devono essere rimosse o sostituite prima che l’e-mail possa essere inviata. Si tratta di un ottimo modo per ricordare agli utenti di aggiungere ulteriore personalizzazione.

Per aggiungere un prompt dei campi, digitare il testo desiderato. Prefettelo con un punto esclamativo e circondatelo con parentesi graffe (vedi sotto).

**Esempi:**

`{{! Introduce yourself}}`

`{{! Insert name of Account Executive}}`

`{{! Add sentence that references their industry and role}}`

<p>Gli utenti dovranno sostituire questo testo con la propria personalizzazione prima di poter inviare l’e-mail.

![](assets/field-prompts-1.png)

>[!NOTE]
>
>Quando si utilizzano i prompt con le campagne di vendita, è consigliabile utilizzarli con passaggi e-mail manuali. Questi passaggi assegnano a un utente un’attività di promemoria per inviare l’e-mail, offrendo l’opportunità di sostituire le richieste con testo personalizzato. Le fasi e-mail automatiche in Campagne di vendita tenteranno di inviare automaticamente, senza consentire all’utente di sostituire le richieste. Se una richiesta non viene sostituita, l’invio delle e-mail non riuscirà.
