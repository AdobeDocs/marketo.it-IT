---
unique-page-id: 14352592
description: Come inserire campi dinamici - Documentazione di Marketo - Documentazione del prodotto
title: Come inserire campi dinamici
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Come inserire campi dinamici {#how-to-insert-dynamic-fields}

Ti consentiamo di personalizzare i modelli e-mail con attributi predefiniti come `{{first_name}}` o `{{company}}`. Questi campi ti consentono di inviare tramite e-mail più contatti e di completarli automaticamente senza doverli digitare separatamente per ciascun contatto.

>[!TIP]
>
>Il campo &quot;first_name&quot; e &quot;company&quot; sono gli unici campi che verranno visualizzati sia in Sales Connect che in Salesforce. Ciò significa che se un contatto non esiste in [applicazione web](https://toutapp.com/login), analizziamo Salesforce per verificare se è possibile trovare un record contatto/lead con un indirizzo e-mail corrispondente. Quindi utilizziamo le informazioni di quel record per compilare il campo.

## Inserire un campo dinamico in un modello {#insert-a-dynamic-field-into-a-template}

1. In entrata **Modelli e campagne**, individua il modello da modificare e fai clic su **Modifica modello**.

1. Clic **Campi dinamici tout**.

   >[!NOTE]
   >
   >Quando si inviano messaggi di posta elettronica a contatti esistenti in Sales Connect, è possibile utilizzare i campi dinamici di base. Questi richiameranno direttamente dal contatto.

Se invii messaggi di posta elettronica a contatti esistenti in Salesforce, puoi sfruttare i campi dinamici di Salesforce. Questi iniziano tutti con &quot;sfdc&quot;. Se disponi di una connessione a Salesforce, questi campi richiameranno direttamente il lead/contatto in Salesforce per compilare le informazioni nel modello.

## Inserire campi dinamici in un oggetto {#insert-dynamic-fields-in-a-subject-line}

È sufficiente copiarli e incollarli manualmente nel campo dell’oggetto di un’e-mail, assicurandosi di disporre della formattazione corretta.
