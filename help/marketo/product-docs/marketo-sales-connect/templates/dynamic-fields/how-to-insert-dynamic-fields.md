---
unique-page-id: 14352592
description: Come inserire campi dinamici - Documenti Marketo - Documentazione prodotto
title: Come inserire campi dinamici
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Come inserire campi dinamici {#how-to-insert-dynamic-fields}

Consentiamo di personalizzare i modelli delle e-mail con attributi predefiniti come `{{first_name}}` o `{{company}}`. Questi campi consentono di inviare più contatti via e-mail e di completare automaticamente questi campi senza dover digitare separatamente per ciascun contatto.

>[!TIP]
>
>I campi &quot;first_name&quot; e &quot;company&quot; sono gli unici campi che verranno visualizzati sia su Sales Connect che su Salesforce. Questo significa che se un contatto non esiste nell&#39; [applicazione Web](https://toutapp.com/login), in Salesforce verificheremo se è possibile trovare un contatto/record lead con un indirizzo e-mail corrispondente. Quindi utilizziamo le informazioni di quel record per compilare il campo.

## Inserire un campo dinamico in un modello {#insert-a-dynamic-field-into-a-template}

1. In **Modelli e campagne**, individua il modello da modificare e fai clic su **Modifica modello**.

1. Fare clic su **Campi dinamici Tout**.

   >[!NOTE]
   >
   >Quando invii tramite e-mail contatti esistenti in Sales Connect, puoi utilizzare i campi dinamici di base. Questi tireranno direttamente dal contatto.

Se invii tramite e-mail contatti esistenti in Salesforce, puoi sfruttare i campi dinamici di Salesforce. Tutto questo inizia con &quot;sfdc&quot;. Se hai una connessione a Salesforce, questi campi richiederanno direttamente al lead/contatto di Salesforce per compilare le informazioni nel modello.

## Inserisci campi dinamici in una riga oggetto {#insert-dynamic-fields-in-a-subject-line}

È sufficiente copiarli e incollarli manualmente nel campo oggetto di un messaggio e-mail, avendo cura di avere la corretta formattazione.
