---
unique-page-id: 14352592
description: Come inserire campi dinamici - Documenti Marketo - Documentazione del prodotto
title: Inserimento di campi dinamici
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Inserimento di campi dinamici {#how-to-insert-dynamic-fields}

Ti consente di personalizzare i modelli e-mail con attributi predefiniti, come `{{first_name}}` o `{{company}}`. Questi campi ti consentono di inviare e-mail a più contatti e completare automaticamente questi campi senza doverli digitare separatamente per ogni contatto.

>[!TIP]
>
>I campi &quot;first_name&quot; e &quot;company&quot; sono gli unici campi che verranno visualizzati sia su Sales Connect che su Salesforce. Ciò significa che se un contatto non esiste nel [applicazione web](https://toutapp.com/login), in Salesforce verifichiamo se è possibile trovare un record contatto/lead con un indirizzo e-mail corrispondente. Quindi utilizziamo le informazioni di quel record per compilare il campo.

## Inserire un campo dinamico in un modello {#insert-a-dynamic-field-into-a-template}

1. In **Modelli e campagne**, trova il modello da modificare e fai clic su **Modifica modello**.

1. Fai clic su **Campi dinamici di Tout**.

   >[!NOTE]
   >
   >Quando invii tramite e-mail contatti esistenti in Sales Connect, puoi utilizzare i campi dinamici di base. Questi tireranno direttamente dal contatto.

Se invii tramite e-mail contatti esistenti in Salesforce, puoi sfruttare i campi dinamici Salesforce. Tutto inizia con &quot;sfdc&quot;. Se si dispone di una connessione a Salesforce, questi campi richiameranno direttamente al lead/contatto di Salesforce per compilare le informazioni nel modello.

## Inserire campi dinamici in una riga oggetto {#insert-dynamic-fields-in-a-subject-line}

È sufficiente copiarli e incollarli manualmente nel campo oggetto di un’e-mail, avendo cura di disporre della formattazione corretta.
