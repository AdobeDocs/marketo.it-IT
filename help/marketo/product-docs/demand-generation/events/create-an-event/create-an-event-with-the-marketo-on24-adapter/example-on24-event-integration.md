---
unique-page-id: 10096679
description: Esempio di integrazione di eventi ON24 - Documentazione di Marketo - Documentazione del prodotto
title: Esempio di integrazione di eventi ON24
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 1%

---

# Esempio di integrazione di eventi ON24 {#example-on-event-integration}

Ecco un evento di esempio, comprese le campagne, per un webinar su ON24. Quando crei l’evento, assicurati di testare le campagne prima di eseguirle.

## Creare un nuovo evento nelle attività di marketing {#create-a-new-event-in-marketing-activities}

1. Seleziona **Nuovo** > **Nuovo programma**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Seleziona un **Cartella campagna** dove si terrà l’evento.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Immetti un **Nome** per l’evento.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Seleziona **Evento** come **Tipo di programma**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Seleziona **Webinar** come **Canale** per l’evento.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Fai clic su **Crea**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Invita (campagna in batch)  {#invite-batch-campaign}

* **Elenco avanzato** : definisci chi invitare all’evento.
* **Flusso**

   * Invia e-mail: se si tratta di un’e-mail di risorsa locale, avrà la seguente convenzione di denominazione: EventName.EmailName. Puoi anche utilizzare le e-mail globali.
   * Modifica stato in Progressione - Imposta su Webinar > Invitato.

* **Pianificazione** - Imposta la data dell&#39;invito da inviare.

## Registrazione/Conferma (Attiva campagna) {#registration-confirmation-trigger-campaign}

* **Elenco avanzato**

   * Attiva la campagna in base a **Compila modulo**. Assicurati di includere la pagina di destinazione in cui si trova il modulo utilizzando **Aggiungi vincolo**, soprattutto se il modulo viene utilizzato su più pagine di destinazione.

>[!CAUTION]
>
>È necessario utilizzare un modulo Marketo per registrare le persone per l’evento oppure un modulo non Marketo con l’integrazione API appropriata per inviare i dati di registrazione a Marketo. Ciò è fondamentale per il successo dell’integrazione con Event Partner. **NOTA**: se utilizzi un modulo Marketo su una pagina di destinazione non Marketo, il trigger sarà **Compila modulo** con il nome del modulo.

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Flusso**

   * **Modifica stato in progressione** - Imposta su Webinar > Registrato. **ATTENZIONE**: questo passaggio di flusso è necessario per configurare la campagna figlio. Quando lo stato di progressione di una persona cambia in **Registrato**, Marketo invia le informazioni di registrazione a ON24.

   * **Invia e-mail** - E-mail di conferma (impostata su **Operativo** in modo che le persone non abbonate che si sono registrate continuino a riceverla).

![](assets/image2015-12-22-15-3a52-3a9.png)

**NOTA**: se la persona viene restituita con un errore di registrazione, non riceverà la conferma e-mail.

## Promemoria (campagna in batch) {#reminder-batch-campaign}

* **Elenco avanzato** - Filtra con **Membro del programma** e imposta lo stato su **Registrato**.

* **Flusso** - Invia e-mail (Promemoria e-mail).

**NOTA**: puoi utilizzare una campagna simile per inviare un *diverso* e-mail di follow-up per gli invitati che non si sono ancora registrati.

## Campagna di follow-up (campagna batch o trigger) {#follow-up-campaign-batch-or-trigger-campaign}

* **Elenco avanzato** - Attivazione in base ai cambiamenti di stato del programma.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Flusso** - Invia e-mail. Utilizza le scelte per inviare e-mail diverse in base allo stato del programma.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[Informazioni sugli eventi delle schede di rete Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
