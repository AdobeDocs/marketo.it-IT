---
unique-page-id: 557339
description: Trovare e unire persone duplicate - Documentazione di Marketo - Documentazione del prodotto
title: Trova e unisci persone duplicate
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
source-git-commit: 780071242a608706e06f3026150c43441a29faa5
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# Trova e unisci persone duplicate {#find-and-merge-duplicate-people}

Marketo esegue automaticamente la deduplicazione quando nuove persone entrano nel sistema. Tuttavia, il CRM potrebbe aver inizialmente inviato duplicati a Marketo. Ecco come unirle.

>[!CAUTION]
>
>L’unione delle persone è permanente, non è possibile annullare l’operazione.

>[!PREREQUISITES]
>
>Per trovare e unire i duplicati è necessario utilizzare [elenchi avanzati incorporati/di sistema](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md).

>[!NOTE]
>
>Marketo non esegue automaticamente la deduplicazione su una sincronizzazione Salesforce o Microsoft Dynamics né quando si immettono manualmente persone.

## Trova duplicati {#find-duplicates}

1. Vai a **Database** area.

   ![](assets/find-and-merge-duplicate-people-1.png)

   >[!CAUTION]
   >
   >L’unione di persone in Marketo potrebbe non funzionare se utilizzi un account Salesforce Person. Unisci i record in Salesforce se possibile.

1. Seleziona la **Possibili duplicati** elenco avanzato di sistema e fare clic sul pulsante **Persone** scheda.

   ![](assets/find-and-merge-duplicate-people-2.png)

   >[!NOTE]
   >
   >È inoltre possibile [Trova persone duplicate con logica personalizzata](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md).

## Unisci persone manualmente {#merge-people-manually}

>[!CAUTION]
>
>Quando si uniscono le persone, se la persona perdente ha un oggetto personalizzato Marketo, **non** vengono riassociate alla persona vincente. Prima di eseguire l&#39;unione, rieseguire l&#39;oggetto personalizzato.

1. Selezionare i duplicati tenendo premuto Ctrl/Comando e facendo clic su, quindi fare clic su **Unisci persone**.

   ![](assets/find-and-merge-duplicate-people-3.png)

   >[!TIP]
   >
   >Potresti avere due o più duplicati per la stessa persona: selezionali tutti contemporaneamente.

1. Verranno visualizzati i valori tra i record che _non_ corrisponde a. Selezionare il valore da mantenere per ogni campo. Clic **Unisci** al termine. Se non desideri entrambi i valori, puoi selezionare **Personalizzato** e inserisci un valore a tua scelta.

   ![](assets/find-and-merge-duplicate-people-4.png)

   >[!NOTE]
   >
   >Quando si uniscono manualmente le persone, la prima persona selezionata sarà il &quot;vincitore&quot;. Quindi, nella scheda Persone, se stai unendo gli ID record 198 e 199 e fai clic su 199 prima, 199 sarà l’ID record delle persone unite. Ciò si applica anche se vengono uniti più di due record.

   >[!TIP]
   >
   >L’unione è migliore dell’eliminazione. Conserverai tutta la cronologia (visite alle pagine, clic sui collegamenti, aperture delle e-mail, riempimenti dei moduli, ecc.).

## Effetto in Salesforce {#effect-in-salesforce}

Se hai integrato Salesforce, ci sono alcune note sull’effetto di Unisci lead in Salesforce.

* Quando si uniscono solo lead o solo contatti, si uniscono in base alle normali regole Salesforce.
* Quando si uniscono lead e contatti, tutti i lead vengono convertiti in contatti prima dell’unione in base alle normali regole di Salesforce.

Per informazioni specifiche sul comportamento di Salesforce durante l’unione di lead o contatti, consulta i seguenti documenti di Salesforce:

* [Unione di lead duplicati](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US)
* [Unione di contatti duplicati](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US)

## Unione in blocco {#bulk-merging}

Se hai troppi duplicati da unire manualmente, contatta l’Adobe Account Team (il tuo Account Manager) per discutere le tue opzioni.

Se sei connesso a un CRM, i record verranno uniti lì in base alle regole seguenti.
