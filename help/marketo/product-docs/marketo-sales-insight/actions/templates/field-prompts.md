---
description: Prompt dei campi - Documentazione di Marketo - Documentazione del prodotto
title: Prompt dei campi
source-git-commit: 7c168abc79e88c9d90786c4d5b86acbc8e0423b6
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

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
