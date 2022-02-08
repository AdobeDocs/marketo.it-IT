---
unique-page-id: 37356194
description: Inviare un elenco a Adobe Experience Cloud - Documentazione Marketo - Documentazione del prodotto
title: Inviare un elenco a Adobe Experience Cloud
exl-id: 770eefe1-05f9-409d-8e7c-b3f1e6ba8139
source-git-commit: a82a2dd0a9c3a27b9b6bf3b352cd81d59932a31b
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Inviare un elenco a Adobe Experience Cloud {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Impossibile utilizzare questa funzionalità in una distribuzione HIPAA di un&#39;istanza Marketo.

>[!PREREQUISITES]
>
>[Configurare la condivisione del pubblico di Adobe Experience Cloud](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)

## Applicazioni di destinazione supportate {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics (**only** se possiedi una licenza Adobe Audience Manager)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe Real-time Customer Data Platform
* Adobe Target

## Come inviare un elenco statico {#how-to-send-a-static-list}

Una lista statica è solo quella, statica. L’elenco in Adobe Experience Cloud non verrà modificato se non manualmente.

1. In Marketo, trova l’elenco da esportare. Fai clic con il pulsante destro del mouse su di esso e seleziona **Invia ad Experience Cloud**.

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. Fai clic sul pulsante **Cartella Audience Manager** e seleziona la cartella di destinazione desiderata nell’Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. Scegli se creare un nuovo pubblico o sovrascriverne uno esistente (in questo esempio ne stiamo creando uno nuovo). Inserisci il nuovo nome del pubblico e fai clic su **Invia**.

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. Fai clic su **OK**.

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

   >[!NOTE]
   >
   >L&#39;iscrizione al pubblico può richiedere fino a 6-8 ore per essere completata in Adobe.

## Come inviare un elenco sincronizzato {#how-to-send-a-synced-list}

La sincronizzazione di un elenco significa che ogni volta che aggiorni un elenco in Marketo, tale modifica si sincronizza automaticamente con il relativo pubblico in Adobe Experience Cloud.

1. In Marketo, trova l’elenco da esportare. Fai clic con il pulsante destro del mouse su di esso e seleziona **Invia ad Experience Cloud**.

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

1. Fai clic sul pulsante **Cartella Libreria Pubblico** e seleziona la cartella di destinazione desiderata nell’Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. Scegli se creare un nuovo pubblico o sovrascriverne uno esistente (in questo esempio ne stiamo creando uno nuovo). Immetti il nuovo nome del pubblico, seleziona il **Mantieni iscrizione pubblico in sincronia** e fai clic su **Invia**.

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. Fai clic su **OK**.

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

## Come interrompere una sincronizzazione elenco {#how-to-stop-a-list-sync}

È possibile impedire la sincronizzazione dell&#39;elenco in qualsiasi momento.

1. In Marketo, trova e fai clic con il pulsante destro del mouse sull’elenco di cui desideri interrompere la sincronizzazione. Fai clic su **Interrompi sincronizzazione elenco**.

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. Seleziona i tipi di pubblico che desideri interrompere la sincronizzazione e fai clic su **Interrompi**.

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

1. Fai clic su **Interrompi** per confermare.

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

## Aspetti da considerare {#things-to-note}

**Condivisione su Adobe Analytics**

Per i clienti che possiedono sia Adobe Audience Manager che Adobe Analytics, questa integrazione consentirà la condivisione dei tipi di pubblico da Marketo alle suite di rapporti di Adobe Analytics. Tuttavia, per abilitarlo, è necessario eseguire alcuni passaggi aggiuntivi in Adobe Audience Manager. Per ulteriori informazioni su come impostare questa configurazione, consulta la documentazione di Adobe Audience Manager: [https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html).

**Utilizzo delle caratteristiche per i clienti Adobe Audience Manager**

Quando avvii un’esportazione di elenchi in Marketo, noterai le seguenti modifiche riportate nell’istanza Adobe Audience Manager:

* Per tutti i lead dell’elenco esportato, Marketo scriverà una caratteristica utilizzando le e-mail con hash dei lead come identificatore tra dispositivi. Il nome della caratteristica corrisponderà al Nome del pubblico di destinazione specificato durante l&#39;esportazione.
* Per tutti gli ECID che Marketo è riuscito a trovare in corrispondenza dei lead nell’elenco esportato, Marketo scriverà una caratteristica utilizzando l’identificatore del dispositivo ECID. Il nome della caratteristica corrisponderà al Nome del pubblico di destinazione specificato durante l&#39;esportazione.
* Marketo creerà anche un segmento nell’istanza di Audience Manager utilizzando la caratteristica ECID come unico criterio di segmentazione. Il nome del segmento corrisponderà al Nome del pubblico di destinazione specificato durante l’esportazione.

## Domande frequenti {#faq}

**Perché la dimensione dell’elenco in Marketo è diversa da quella dell’Adobe?**

Sotto il cofano, l&#39;integrazione del pubblico funziona sincronizzando i cookie Marketo Munchkin con il cookie ECID Adobe corrispondente. Marketo può condividere i dati di iscrizione solo per i lead per i quali Marketo ha sincronizzato un ECID. Per ottenere i migliori risultati possibili, ti consigliamo di caricare lo script di tracciamento munchkin.js di Marketo in parallelo con il codice di tracciamento visitor.js di Adobe su tutte le pagine che desideri tracciare a scopo di marketing.

**Come funziona la sincronizzazione dei cookie?**

Quando la sincronizzazione dei cookie è abilitata per la tua iscrizione Marketo, Marketo’s munchkin.js tenterà di acquisire e memorizzare gli ECID Adobi per l’organizzazione Adobe IMS specificata durante la configurazione dell’integrazione e di far corrispondere questi ECID all’identificatore cookie Marketo corrispondente. Questo consente ai profili utente anonimi di Marketo di arricchirsi di ECID Adobi.

È necessario un ulteriore passaggio per associare il profilo utente anonimo a un profilo lead, identificato utilizzando un messaggio e-mail di testo normale. Esattamente come funziona [qui descritto](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md).

**Quali informazioni sono condivise?**

Questa integrazione condivide solo le informazioni sull’appartenenza all’elenco da Marketo all’Adobe (ad esempio, se lead X è membro dell’elenco Y). Nessun attributo lead aggiuntivo viene condiviso in Adobe tramite questa integrazione.
