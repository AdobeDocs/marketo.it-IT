---
unique-page-id: 37356194
description: Inviare un elenco a Adobe Experience Cloud - Documentazione Marketo - Documentazione del prodotto
title: Inviare un elenco a Adobe Experience Cloud
exl-id: 770eefe1-05f9-409d-8e7c-b3f1e6ba8139
feature: Static Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 1%

---

# Inviare un elenco a Adobe Experience Cloud {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Una distribuzione compatibile con HIPAA di un’istanza Marketo non può utilizzare questa funzione.

>[!PREREQUISITES]
>
>[Imposta mapping organizzazione Adobe](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Applicazioni di destinazione supportate {#supported-destination-applications}

* Adobe Advertising Cloud
* ADOBE ANALYTICS (**solo** se possiedi una licenza Adobe Audience Manager)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe Real-time Customer Data Platform
* Adobe Target

## Come inviare un elenco statico {#how-to-send-a-static-list}

Un elenco statico è solo questo, statico. Non verrà apportata alcuna modifica all&#39;elenco in Adobe Experience Cloud, a meno che non vengano apportate manualmente.

1. In Marketo, individua l’elenco da esportare. Fai clic con il pulsante destro del mouse e seleziona (Confronta periodi di tempo) **Invia all’Experience Cloud**.

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. Fai clic su **Cartella Audience Manager** e selezionare la cartella di destinazione desiderata nell’Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. Scegli se creare un nuovo pubblico o sovrascriverne uno esistente (in questo esempio ne stiamo creando uno nuovo). Inserisci il nuovo nome del pubblico e fai clic su **Invia**.

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. Clic **OK**.

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

   >[!NOTE]
   >
   >Possono essere necessarie fino a 6-8 ore affinché l’iscrizione al pubblico possa essere completamente popolata in Adobe.

## Come inviare un elenco sincronizzato {#how-to-send-a-synced-list}

La sincronizzazione di un elenco significa che ogni volta che si aggiorna un elenco in Marketo, la modifica viene automaticamente sincronizzata con il relativo pubblico in Adobe Experience Cloud.

1. In Marketo, individua l’elenco da esportare. Fai clic con il pulsante destro del mouse e seleziona (Confronta periodi di tempo) **Invia all’Experience Cloud**.

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

1. Fai clic su **Cartella libreria Pubblico** e selezionare la cartella di destinazione desiderata nell’Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. Scegli se creare un nuovo pubblico o sovrascriverne uno esistente (in questo esempio ne stiamo creando uno nuovo). Immetti il nuovo nome del pubblico, seleziona la **Mantieni appartenenza pubblico sincronizzata** e fare clic su **Invia**.

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. Clic **OK**.

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

## Interrompere una sincronizzazione elenco {#how-to-stop-a-list-sync}

Puoi interrompere la sincronizzazione dell’elenco in qualsiasi momento.

1. In Marketo, individua e fai clic con il pulsante destro del mouse sull’elenco che desideri interrompere la sincronizzazione. Clic **Interrompi sincronizzazione elenco**.

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. Seleziona i tipi di pubblico che desideri interrompere e fai clic su **Interrompi**.

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

1. Clic **Interrompi** per confermare.

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

## Aspetti da considerare {#things-to-note}

**Condivisione con Adobe Analytics**

Per i clienti che possiedono sia Adobe Audience Manager che Adobe Analytics, questa integrazione consentirà ai tipi di pubblico di essere condivisi da Marketo alle suite di rapporti di Adobe Analytics. Tuttavia, è necessario seguire alcuni passaggi di configurazione aggiuntivi in Adobe Audience Manager per abilitare questa funzione. Per ulteriori informazioni su come impostare questa configurazione, consulta la documentazione di Adobe Audience Manager: [https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html).

**Utilizzo delle caratteristiche per i clienti Adobe Audience Manager**

Quando avvii un’esportazione di elenchi in Marketo, noterai le seguenti modifiche riportate nell’istanza di Adobe Audience Manager:

* Per tutti i lead nell’elenco esportato, Marketo scriverà una caratteristica utilizzando le e-mail con hash dei lead come identificatore multi-dispositivo. Il nome della caratteristica corrisponderà al Nome del pubblico di destinazione specificato durante l’esportazione.
* Per tutti gli ECID che Marketo è riuscito a trovare corrispondenti ai lead nell’elenco esportato, Marketo scriverà una caratteristica utilizzando l’identificatore del dispositivo ECID. Il nome della caratteristica corrisponderà al Nome del pubblico di destinazione specificato durante l’esportazione.
* Marketo creerà anche un segmento nell’istanza dell’Audience Manager utilizzando la caratteristica ECID come unico criterio di segmentazione. Il nome del segmento corrisponderà al Nome del pubblico di destinazione specificato durante l’esportazione.

## Domande frequenti {#faq}

**Perché la dimensione dell’elenco in Marketo è diversa da quella in Adobe?**

Dal punto di vista tecnico, l’integrazione del pubblico funziona sincronizzando i cookie di Marketo Munchkin con il cookie ECID di Adobe corrispondente. Marketo può condividere solo i dati di iscrizione per i lead per i quali Marketo ha sincronizzato un ECID. Per ottenere i migliori risultati possibili, ti consigliamo di caricare lo script di tracciamento munchkin.js di Marketo in parallelo al codice di tracciamento visitor.js di Adobe su tutte le pagine che ti interessano a scopo di marketing.

**Come funziona la sincronizzazione dei cookie?**

Quando la sincronizzazione dei cookie è abilitata per l’abbonamento a Marketo, munchkin.js di Marketo tenterà di acquisire e memorizzare gli ECID di Adobe per l’organizzazione IMS di Adobe specificata durante la configurazione dell’integrazione e far corrispondere questi ECID all’identificatore cookie di Marketo corrispondente. Questo consente ai profili utente anonimi di Marketo di arricchirsi di ECID Adobi.

È necessario un ulteriore passaggio per associare il profilo utente anonimo a un profilo lead, identificato utilizzando un’e-mail in testo normale. Esattamente come funziona questo [descritto qui](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md).

**Quali informazioni vengono condivise?**

Questa integrazione condivide solo le informazioni sull’iscrizione all’elenco da Marketo a Adobe (ad esempio, sapendo che il lead X è membro dell’elenco Y). Tramite questa integrazione, nessun attributo lead aggiuntivo viene condiviso con Adobe.
