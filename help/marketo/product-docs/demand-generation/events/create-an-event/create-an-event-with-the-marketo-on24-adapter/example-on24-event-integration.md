---
unique-page-id: 10096679
description: Esempio di integrazione di eventi ON24 - Documentazione di Marketo - Documentazione del prodotto
title: Esempio di integrazione di eventi ON24
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 2%

---

# Esempio di integrazione di eventi ON24 {#example-on-event-integration}

Ecco un evento di esempio, comprese le campagne, per un webinar su ON24. Quando crei l’evento, assicurati di testare le campagne prima di eseguirle.

## Creare un nuovo evento nelle attività di marketing {#create-a-new-event-in-marketing-activities}

1. Selezionare **[!UICONTROL New]** > **[!UICONTROL New Program]**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Seleziona un **[!UICONTROL Campaign Folder]** in cui vivrà l&#39;evento.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Immetti **[!UICONTROL Name]** per l&#39;evento.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Seleziona **[!UICONTROL Event]** come **[!UICONTROL Program Type]**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Selezionare **[!UICONTROL Webinar]** come **[!UICONTROL Channel]** per l&#39;evento.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Fai clic su **[!UICONTROL Create]**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Invita (campagna in batch)  {#invite-batch-campaign}

* **Elenco avanzato** - Definisci chi invitare all&#39;evento.
* **Flusso**

   * Invia e-mail: se si tratta di un’e-mail di risorsa locale, avrà la seguente convenzione di denominazione: EventName.EmailName. Puoi anche utilizzare le e-mail globali.
   * Modifica stato in Progressione - Imposta su Webinar > Invitato.

* **Pianificazione** - Imposta la data dell&#39;invito da inviare.

## Registrazione/Conferma (Attiva campagna) {#registration-confirmation-trigger-campaign}

* **Elenco avanzato**

   * Attiva la campagna in base a **[!UICONTROL Fills Out Form]**. Assicurarsi di includere la pagina di destinazione in cui si trova il modulo utilizzando **[!UICONTROL Add Constraint]**, soprattutto se il modulo viene utilizzato su più pagine di destinazione.

>[!CAUTION]
>
>È necessario utilizzare un modulo Marketo per registrare le persone per l’evento oppure un modulo non Marketo con l’integrazione API appropriata per inviare i dati di registrazione a Marketo. Questo è fondamentale per il successo dell&#39;integrazione di [!UICONTROL Event Partner]. **NOTA**: se si utilizza un modulo Marketo in una pagina di destinazione non Marketo, il trigger sarà **[!UICONTROL Fills Out Form]** con [!UICONTROL Form Name].

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Flusso**

   * **Modifica stato in progressione** - Imposta su Webinar > Registrato. **ATTENZIONE**: questo passaggio di flusso è obbligatorio durante la configurazione della campagna secondaria. Quando lo stato di progressione di una persona cambia in **Registrato**, Marketo invia le informazioni di registrazione a ON24.

   * **Invia e-mail** - E-mail di conferma (impostata su **Operativa** in modo che le persone non abbonate che si sono registrate continuino a riceverla).

![](assets/image2015-12-22-15-3a52-3a9.png)

**NOTA**: se la persona viene restituita con un errore di registrazione, non riceverà la conferma e-mail.

## Promemoria (campagna in batch) {#reminder-batch-campaign}

* **Elenco avanzato** - Filtra utilizzando **Membro del programma** e imposta lo stato su **Registrato**.

* **Flusso** - Invia e-mail (Promemoria e-mail).

**NOTA**: è possibile utilizzare una campagna simile per inviare un messaggio e-mail di follow-up *diverso* a persone invitate ma non ancora registrate.

## Campagna di follow-up (campagna batch o trigger) {#follow-up-campaign-batch-or-trigger-campaign}

* **Elenco avanzato** - Attivazione basata su modifiche dello stato del programma.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Flusso** - Invia e-mail. Utilizza le scelte per inviare e-mail diverse in base allo stato del programma.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[Informazioni sugli eventi della scheda di rete Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
