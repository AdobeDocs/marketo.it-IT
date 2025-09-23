---
unique-page-id: 18317340
description: Verifica annullamento iscrizione Marketo - Documentazione Marketo - Documentazione del prodotto
title: Verificare l’annullamento dell’iscrizione Marketo
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 5%

---

# Verificare l’annullamento dell’iscrizione Marketo {#marketo-unsubscribe-check}

[!UICONTROL Marketo Unsubscribe Check] utilizza la connessione del tuo team a Marketo per impedire che le e-mail arrivino a persone non iscritte al sistema di gestione dei lead di Marketo. Quando un utente di vendita invia un&#39;e-mail con [!DNL Sales Connect], verrà effettuata una chiamata API a Marketo per verificare se l&#39;ID e-mail non è abbonato. In caso affermativo, l’e-mail non verrà inviata.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Attivazione {#turning-it-on}

1. Nell&#39;applicazione Web fare clic sull&#39;icona a forma di ingranaggio e selezionare **[!UICONTROL Settings]**.

   ![](assets/one-2.png)

1. In [!UICONTROL Admin Settings], fare clic su **[!UICONTROL Unsubscribes]**.

   ![](assets/two-3.png)

1. Fai clic su **[!UICONTROL Integrations]**.

   ![](assets/three-3.png)

1. Nella sezione [!UICONTROL Marketo Unsubscribe Check], fare clic sul dispositivo di scorrimento per attivare il controllo.

   ![](assets/four-2.png)

## Aspetti da comprendere {#things-to-know}

Controllo per annullare l’abbonamento a Marketo...

* Non viene conteggiato rispetto ai limiti API
* Richiede la connessione a Marketo
* È un’impostazione globale
* Blocca le e-mail inviate dall’applicazione web, dai client e-mail e da Salesforce
* Registrerà un messaggio e-mail non riuscito o impedirà a un utente di inviarlo quando tenta di inviare per tutti i flussi di lavoro (invio del plug-in e-mail, invio di singoli utenti, invio della campagna di vendita, selezione multipla e invio) ad eccezione di [e-mail di gruppo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md), in cui impediremo l&#39;invio silenzioso dei messaggi e-mail
