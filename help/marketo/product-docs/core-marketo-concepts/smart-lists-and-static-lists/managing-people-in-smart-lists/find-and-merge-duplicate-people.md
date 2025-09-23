---
unique-page-id: 557339
description: Trovare e unire persone duplicate - Documentazione di Marketo - Documentazione del prodotto
title: Trovare e unire persone duplicate
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 3%

---

# Trovare e unire persone duplicate {#find-and-merge-duplicate-people}

Marketo Engage esegue automaticamente la deduplicazione quando nuove persone entrano nel sistema. Tuttavia, il CRM potrebbe inizialmente aver inviato più duplicati. Ecco come unirle.

>[!CAUTION]
>
>L’unione delle persone è permanente, non è possibile annullare l’operazione.

>[!PREREQUISITES]
>
>Per trovare e unire i duplicati è necessario utilizzare [elenchi smart incorporati/di sistema](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md){target="_blank"}.

>[!NOTE]
>
>Marketo non eseguirà la deduplicazione automatica in base a una sincronizzazione [!DNL Salesforce] o [!DNL Microsoft Dynamics] o quando si immettono manualmente persone.

## Trova duplicati {#find-duplicates}

1. Passa alla schermata **[!UICONTROL Database]**.

   ![](assets/find-and-merge-duplicate-people-1.png)

   >[!CAUTION]
   >
   >L&#39;unione di persone in Marketo potrebbe non funzionare se si utilizza un account persona [!DNL Salesforce]. Unisci i record in [!DNL Salesforce] se possibile.

1. Selezionare l&#39;elenco avanzato di sistema **[!UICONTROL Possible Duplicates]** e fare clic sulla scheda **[!UICONTROL People]**.

   ![](assets/find-and-merge-duplicate-people-2.png)

   >[!NOTE]
   >
   >Puoi anche [Trovare persone duplicate con logica personalizzata](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md){target="_blank"}.

## Unisci persone manualmente {#merge-people-manually}

>[!CAUTION]
>
>Durante l&#39;unione delle persone, se la persona perdente ha un oggetto personalizzato Marketo, _non_ verrà nuovamente associata alla persona vincente. Prima di eseguire l&#39;unione, rieseguire l&#39;oggetto personalizzato.

1. Selezionare i duplicati tenendo premuto Ctrl/Comando e facendo clic su, quindi fare clic su **[!UICONTROL Merge People]**.

   ![](assets/find-and-merge-duplicate-people-3.png)

   >[!TIP]
   >
   >Potresti avere due o più duplicati per la stessa persona: selezionali tutti contemporaneamente.

1. Vedrai i valori tra i record che _non_ corrispondono. Selezionare il valore da mantenere per ogni campo. Al termine, fai clic su **[!UICONTROL Merge]**. Se non si desidera utilizzare nessuno dei due valori, è possibile selezionare **[!UICONTROL Custom]** e immettere un valore desiderato.

   ![](assets/find-and-merge-duplicate-people-4.png)

   >[!NOTE]
   >
   >Quando si uniscono manualmente le persone, la prima persona selezionata sarà il &quot;vincitore&quot;. Quindi, nella scheda Persone, se stai unendo gli ID record 198 e 199 e fai clic su 199 prima, 199 sarà l’ID record delle persone unite. Ciò si applica anche se vengono uniti più di due record.

   >[!TIP]
   >
   >L’unione è migliore dell’eliminazione. Conserverai tutta la cronologia (visite alle pagine, clic sui collegamenti, aperture delle e-mail, riempimenti dei moduli, ecc.).

## Effetto in Salesforce {#effect-in-salesforce}

Se hai integrato Salesforce, ci sono alcune note sull’effetto dell’unione di lead in Salesforce.

* Quando si uniscono solo lead o solo contatti, vengono uniti in base alle normali regole [!DNL Salesforce].
* Quando si uniscono lead e contatti, tutti i lead vengono convertiti in contatti prima dell&#39;unione in base alle normali regole [!DNL Salesforce].

Per informazioni specifiche sul comportamento di Salesforce durante l&#39;unione di lead o contatti, controllare i seguenti [!DNL Salesforce] documenti:

* [Unione di lead duplicati](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&language=en_US){target="_blank"}
* [Unione di contatti duplicati](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&language=en_US){target="_blank"}

## Unione in blocco {#bulk-merging}

Se hai troppi duplicati da unire manualmente, contatta il team dell’account di Adobe (il tuo Account Manager) per discutere le tue opzioni.
