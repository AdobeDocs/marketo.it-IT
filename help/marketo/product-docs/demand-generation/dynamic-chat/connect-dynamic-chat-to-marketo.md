---
description: Collegare la chat dinamica a Marketo - Documentazione Marketo - Documentazione del prodotto
title: Collegare la chat dinamica a Marketo
exl-id: bad6c2dc-d4e7-4f98-bf6d-743043f96e4e
source-git-commit: 9b49c9f0ee03ab72672f46618fb24eed174bf835
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Collegare la chat dinamica a Marketo {#connect-dynamic-chat-to-marketo}

Dopo aver completato le [configurazione iniziale](/help/marketo/product-docs/demand-generation/dynamic-chat/initial-setup.md), è il momento di eseguire la sincronizzazione una tantum collegando la chat dinamica al tuo abbonamento Marketo.

1. In My Marketo, fai clic sul pulsante **Chat dinamica** piastrelle.

   ![](assets/connect-dynamic-chat-to-marketo-1.png)

   >[!NOTE]
   >
   >Se non trovi la tessera , contatta il tuo amministratore Marketo.

1. Se in precedenza hai effettuato l’accesso a un’applicazione con un Adobe ID, verrai reindirizzato direttamente a Chat dinamico. In caso contrario, [configurare il tuo Adobe ID](https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html).

1. Per collegare l’istanza Marketo, seleziona **Integrazioni**.

   ![](assets/connect-dynamic-chat-to-marketo-2.png)

1. Nella scheda Marketo, fai clic su **Avvia sincronizzazione**.

   ![](assets/connect-dynamic-chat-to-marketo-3.png)

1. Seleziona fino a 50 campi standard o personalizzati dall’istanza di Marketo per la sincronizzazione con la chat dinamica da utilizzare nel targeting del pubblico, nella mappatura dei dati e nella personalizzazione. Fai clic su **Successivo** al termine.

   ![](assets/connect-dynamic-chat-to-marketo-4.png)

   >[!CAUTION]
   >
   >Al momento, le selezioni degli attributi **impossibile** vengono modificati dopo la sincronizzazione iniziale. Al termine della sincronizzazione, puoi solo tornare indietro e aggiungere di più (se hai scelto meno di 50).

1. Rivedi le selezioni (promemoria: non è possibile rimuovere gli attributi post-sincronizzazione, quindi fai clic su **Modifica selezioni** se devi modificare qualcuno in questo passaggio). Fai clic su **Conferma** al termine dell’avvio della sincronizzazione.

   ![](assets/connect-dynamic-chat-to-marketo-5.png)

>[!NOTE]
>
>Il completamento della sincronizzazione può richiedere da 2 a 24 ore, a seconda delle dimensioni del database.

## Collega la tua organizzazione Adobe e Marketo {#link-your-adobe-org-and-marketo}

Ora è il momento di collegare Adobe e Marketo.

1. Accedi a [experience.adobe.com](https://experience.adobe.com).

1. Fare clic sullo schermo in un punto qualsiasi dell&#39;Experience Cloud e premere ctrl+i. In **Organizzazioni assegnate** , evidenzia e copia l&#39;ID organizzazione (_meno_ &quot;@AdobeOrg&quot;). Press **Chiudi** al termine.

   ![](assets/connect-dynamic-chat-to-marketo-6.png)

1. In Marketo, vai alla pagina **Amministratore** e seleziona **Mappatura dell&#39;organizzazione di Adobe**.

   ![](assets/connect-dynamic-chat-to-marketo-7.png)

1. Fai clic su **Modifica**.

   ![](assets/connect-dynamic-chat-to-marketo-8.png)

1. Incolla l’ID organizzazione copiato al passaggio 2 e fai clic su **OK**.

   ![](assets/connect-dynamic-chat-to-marketo-9.png)

>[!MORELIKETHIS]
>
>[Configurazione iniziale](/help/marketo/product-docs/demand-generation/dynamic-chat/initial-setup.md)
