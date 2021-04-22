---
unique-page-id: 557339
description: Trova e unisci persone duplicate - Documenti Marketo - Documentazione del prodotto
title: Trova e unisci persone duplicate
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Trova e unisci persone duplicate {#find-and-merge-duplicate-people}

Marketo deduplica automaticamente quando nuove persone accedono al sistema. Tuttavia, il tuo CRM potrebbe aver inizialmente inviato duplicati a Marketo. Ecco come fonderle.

>[!NOTE]
>
>Marketo non eseguirà la deduplicazione automatica contro una sincronizzazione Salesforce o Microsoft Dynamics o quando si immettono manualmente le persone.

>[!PREREQUISITES]
>
>La ricerca e l&#39;unione di duplicati richiederà l&#39;utilizzo di [elenchi smart incorporati / di sistema](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md).

## Trova duplicati {#find-duplicates}

1. Passa all&#39;area **Database**.

   ![](assets/db.png)

   >[!CAUTION]
   >
   >L’unione delle persone in Marketo potrebbe non funzionare se utilizzi un account personale Salesforce. Unisci i record in Salesforce, se possibile.

1. Seleziona l&#39;elenco smart di sistema **Duplicati possibili** e fai clic sulla scheda **Persone** .

   ![](assets/two.png)

   >[!NOTE]
   >
   >Puoi anche [trovare persone duplicate con logica personalizzata](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md).

## Unisci manualmente le persone {#merge-people-manually}

>[!CAUTION]
>
>Durante l&#39;unione delle persone, se la persona perdente ha un oggetto personalizzato Marketo, **non** verrà riassociata alla persona vincente. Prima di eseguire l&#39;unione, rieseguire l&#39;oggetto personalizzato.

1. Seleziona i duplicati tenendo premuto Ctrl/Comando e facendo clic su , quindi fai clic su **Unisci persone**.

   ![](assets/three.png)

   >[!TIP]
   >
   >Potresti avere due o più duplicati per la stessa persona - selezionali tutti contemporaneamente.

1. Vedrai i valori tra i record che _non_ corrispondono. Selezionare il valore da mantenere per ogni campo. Al termine, fai clic su **Unisci**. Se non desideri entrambi i valori, puoi selezionare **Personalizzato** e immettere un valore desiderato.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Quando si uniscono manualmente le persone, la prima persona selezionata sarà &quot;vincitrice&quot;. Quindi nella scheda Persone se unisci ID record 198 e 199 e fai clic prima sul 199, 199 sarà l&#39;ID record delle persone unite. Questo vale anche se vengono uniti più di due record.

   >[!TIP]
   >
   >L&#39;unione è meglio dell&#39;eliminazione. Conserverai tutta la cronologia (visite alle pagine, clic sui collegamenti, aperture delle e-mail, riempimenti dei moduli, ecc.).

## Effetto Salesforce {#effect-in-salesforce}

Se disponi dell’integrazione Salesforce, ci sono alcune note sull’effetto di Unisci lead in Salesforce.

* Quando si uniscono solo i Lead o solo i Contatti, si uniscono in base alle normali regole di Salesforce.
* Durante l&#39;unione di Lead e Contatti, tutti i Lead vengono convertiti in Contatti prima dell&#39;unione in base alle normali regole Salesforce.

Per informazioni specifiche sul comportamento di Salesforce durante l&#39;unione di Lead o Contatti, controlla i seguenti documenti Salesforce:

* [Unione di lead duplicati](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US)
* [Unione di contatti duplicati](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US)

## Unione in blocco {#bulk-merging}

Se hai troppi duplicati da unire manualmente, contatta il tuo Customer Success Manager per discutere le tue opzioni.

Super! Se sei connesso a un CRM, i record verranno uniti in base alle regole riportate di seguito.
