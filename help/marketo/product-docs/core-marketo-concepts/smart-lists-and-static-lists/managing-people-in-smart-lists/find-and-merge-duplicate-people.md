---
unique-page-id: 557339
description: Trova e unisci persone duplicate - Documenti Marketo - Documentazione prodotto
title: Trova e unisci persone duplicate
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 0%

---


# Trova e unisci persone duplicate {#find-and-merge-duplicate-people}

Marketo deduplica automaticamente quando nuove persone entrano nel sistema. Tuttavia, il CRM potrebbe aver inizialmente inviato duplicati a Marketo. Ecco come fonderli.

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

>[!NOTE]
>
>Marketo non eseguirà automaticamente la deduplicazione rispetto a una sincronizzazione Salesforce o Microsoft Dynamics, o quando immetti manualmente le persone.

>[!PREREQUISITES]
>
>La ricerca e l&#39;unione di duplicati implica l&#39;utilizzo di elenchi [intelligenti](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md)integrati/di sistema.

## Trova duplicati {#find-duplicates}

1. Passare all&#39;area **Database** .

   ![](assets/db.png)

   >[!CAUTION]
   >
   >L&#39;unione di persone in Marketo potrebbe non funzionare se utilizzi un account Salesforce Person. Unisci i record in Salesforce, se possibile.

1. Selezionate l&#39;elenco smart **Possibile** sistema **Duplicati** e fate clic sulla scheda **Persone** .

   ![](assets/two.png)

   >[!NOTE]
   >
   >È inoltre possibile [trovare persone duplicate con logica](find-duplicate-people-with-custom-logic.md)personalizzata.

## Unisci manualmente le persone {#merge-people-manually}

>[!CAUTION]
>
>Durante l&#39;unione delle persone, se la persona perdente ha un oggetto personalizzato Marketo, **non** verrà riassociata alla persona vincente. Eseguire nuovamente l&#39;oggetto personalizzato prima di eseguire l&#39;unione.

Per selezionare i duplicati, tenete premuto Ctrl/Comando e fate clic su Unisci persone.
![](assets/three.png)

>[!TIP]
>
>È possibile avere due o più duplicati per la stessa persona, selezionarli tutti contemporaneamente.

1. Verranno visualizzati i valori tra i record che *non* corrispondono. Selezionare il valore da mantenere per ciascun campo. Al termine, fate clic su **Unisci** . Se non si desidera alcun valore, è possibile selezionare **Personalizzato** e immettere un valore di propria scelta.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Quando si uniscono manualmente le persone, la prima persona selezionata sarà &quot;vincente&quot;. Quindi nella scheda Persone se state unendo gli ID record 198 e 199, e per caso fate clic sul 199 prima, 1999 sarà l&#39;ID record delle persone unite. Ciò vale anche se vengono uniti più di due record.

   >[!TIP]
   >
   >L&#39;unione è meglio che eliminare. Conservate tutta la cronologia (visite delle pagine, clic sui collegamenti, apertura delle e-mail, riempimenti dei moduli, ecc.).

## Effetto in Salesforce {#effect-in-salesforce}

Se disponete dell&#39;integrazione Salesforce, potete trovare alcune note sull&#39;effetto di Unisci lead in Salesforce.

    * Quando si uniscono solo i lead o solo i contatti, si uniscono in base alle normali regole di Salesforce.
    * Durante l&#39;unione di lead e contatti, tutti i lead vengono convertiti in contatti prima dell&#39;unione in base alle normali regole di Salesforce.

Per informazioni specifiche sul comportamento di Salesforce durante l&#39;unione di lead o contatti, consulta i seguenti documenti Salesforce:

    * [Unione di lead duplicati](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US)
    * [Unione di contatti duplicati](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US)

## Unione in blocco {#bulk-merging}

Se hai troppi duplicati da unire manualmente, contatta il tuo Customer Success Manager per conoscere le tue opzioni.

Super! Se sei connesso a un CRM, i record verranno uniti in base alle regole riportate di seguito.