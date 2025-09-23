---
description: Prompt dei campi - Documentazione di Marketo - Documentazione del prodotto
title: Prompt dei campi
exl-id: c138b627-f853-4d35-b022-cc517d6b86d4
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 3%

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
>Quando si utilizzano i prompt con le campagne di vendita, è consigliabile utilizzarli con i passaggi manuali dell’e-mail. Questi passaggi assegnano a un utente un’attività di promemoria per inviare l’e-mail, offrendo l’opportunità di sostituire le richieste con testo personalizzato. Le fasi e-mail automatiche in Campagne di vendita tenteranno di inviare automaticamente, senza consentire all’utente di sostituire le richieste. Se una richiesta non viene sostituita, l’invio delle e-mail non riuscirà.
