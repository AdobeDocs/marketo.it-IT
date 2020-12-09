---
unique-page-id: 10096679
description: Esempio di integrazione degli eventi ON24 - Documenti Marketo - Documentazione del prodotto
title: Esempio di integrazione evento ON24
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# Esempio di integrazione evento ON24 {#example-on-event-integration}

Ecco un esempio di evento, incluse le campagne, per un webinar ON24. Quando create un evento, accertatevi di verificare le campagne prima di eseguirle.

## Creazione di un nuovo evento nelle attività di marketing {#create-a-new-event-in-marketing-activities}

1. Selezionare **Nuovo** > **Nuovo programma**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Selezionate una cartella **di** campagna in cui l&#39;evento vivrà.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Immettete un **nome** per l’evento.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Selezionare **Event **come tipo **di** programma.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Selezionare **Webinar **come **Canale **per l&#39;evento.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Fate clic su **Crea**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Invita (campagna batch)  {#invite-batch-campaign}

* **Elenco** avanzato - Consente di definire gli invitati all’evento.
* **Flusso**

   * Invia e-mail: se si tratta di un messaggio e-mail di risorsa locale, avrà la seguente convenzione di denominazione: EventName.EmailName. Potete anche utilizzare e-mail globali.
   * Modifica stato in progressione - Impostate su Webinar > Invitato.

* **Pianificazione** - Imposta la data per l&#39;invio dell&#39;invito.

## Registrazione/conferma (Trigger Campaign) {#registration-confirmation-trigger-campaign}

* **Smart List**

   * Attiva la campagna in base al **modulo** di compilazione. Accertarsi di includere la pagina di destinazione su cui si trova il modulo utilizzando **Aggiungi vincolo**, in particolare se il modulo è utilizzato su più pagine di destinazione.

>[!CAUTION]
>
>È necessario utilizzare un modulo Marketo per registrare le persone per l&#39;evento, oppure un modulo non Marketo con l&#39;integrazione API corretta per inviare i dati di registrazione push a Marketo. Ciò è fondamentale per il successo dell&#39;integrazione dei partner evento. **NOTA**: Se si utilizza un modulo Marketo su una pagina di destinazione non Marketo, viene attivato **Compilazione del modulo** con il nome del modulo.

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Flusso**

   * **Modifica stato in progressione** - Impostate su Webinar > Registrato. **ATTENZIONE**: Questo passaggio di flusso è necessario per configurare la campagna figlio. Quando lo stato di progressione di una persona cambia in **Registrato**, Marketo invia le informazioni di registrazione a ON24.

   * **Invia e-mail** - Messaggio e-mail di conferma (impostato su **Operativo** in modo che gli utenti non iscritti che si sono registrati lo ricevano ancora).

![](assets/image2015-12-22-15-3a52-3a9.png)

**NOTA**: Se la persona viene restituita con un errore di registrazione, non riceverà la conferma e-mail.

## Promemoria (campagna batch) {#reminder-batch-campaign}

* **Smart List** - Filtrare utilizzando **Member of Program** e impostare lo stato su **Registered**.

* **Flusso** - Invia e-mail (e-mail promemoria).

**NOTA**: Potete utilizzare una campagna simile per inviare un&#39;e-mail di follow-up *diversa* alle persone invitate ma che non si sono ancora registrate.

## Campagna di follow-up (Batch o Trigger Campaign) {#follow-up-campaign-batch-or-trigger-campaign}

* **Smart List** - Trigger in base alle modifiche dello stato del programma.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Flusso** - Invia e-mail. Usa le opzioni per inviare e-mail diverse in base allo stato del programma.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>* [Informazioni sugli eventi dell&#39;adattatore Marketo ON24](understanding-marketo-on24-adapter-events.md)

>



