---
unique-page-id: 11379045
description: Aggiungere un passaggio di flusso per SMS - Marketo Docs - Documentazione prodotto
title: Aggiunta di un passaggio di flusso per SMS
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# Aggiungere un passaggio di flusso per SMS {#add-a-flow-step-for-sms}

Marketo ha tre passaggi di flusso che puoi utilizzare nelle tue campagne smart SMS:

* **Invia messaggio**  SMS - Questa azione di flusso invia messaggi alle persone dall&#39;elenco di smartlist Marketo sottoscritte da un elenco di iscrizione Vibes selezionato dall&#39;utente. Non avvia il processo di iscrizione.
* **Iscrizione a elenco**  vibrazioni: questa azione di flusso avvia il processo di iscrizione SMS tramite una campagna di acquisizione Vibes selezionata dall&#39;utente. Vibes invia quindi un messaggio di conferma; il destinatario deve rispondere per completare la procedura di iscrizione.
* **Annulla sottoscrizione a elenco**  vibrazioni: questa azione di flusso annulla la sottoscrizione a ogni utente da un elenco di iscrizioni Vibes selezionato dall&#39;utente.

>[!NOTE]
>
>Quando si inviano messaggi SMS:
>
>* Marketo dedupe per numero di telefono. Quindi se più persone hanno lo stesso numero di telefono, solo una persona riceverà il messaggio.
>* Marketo non invierà a persone  inserire nell&#39;elenco Bloccati o Sospese di marketing.


Per informazioni generali sulla configurazione dei passaggi di flusso, vedere [Aggiungi un passaggio di flusso a una campagna intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Queste sono le basi per l&#39;utilizzo di SMS.

1. In My Marketo, fate clic su **Marketing Activities**.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. Trova la campagna intelligente a cui vuoi aggiungere il flusso di SMS. Fare clic sulla scheda **Flusso**.

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. Trascinare sul flusso, ad esempio **Invia messaggio SMS**. Seleziona SMS Message (Messaggio SMS) e l&#39;elenco Vibes (Vibrazioni) dall&#39;elenco a discesa.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Il selettore Elenco variabili funge da ulteriore filtro per l&#39;audience già identificata nell&#39;elenco avanzato, per eseguire il targeting dei soli lead che appartengono a tale elenco Vibes.
   >
   >I flussi **Iscrizione a Vibes List** e **Annulla sottoscrizione a Vibes List** hanno requisiti diversi. Per **Iscrizione**, devi selezionare l&#39;elenco Vibes e la campagna di acquisizione Vibes. Per **Annulla sottoscrizione**, è richiesto solo l&#39;elenco Vibes.
