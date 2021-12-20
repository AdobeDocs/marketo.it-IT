---
description: Inviare un segmento Adobe Experience Platform a un elenco statico di Marketo - Documenti Marketo - Documentazione del prodotto
title: Inviare un segmento Adobe Experience Platform a un elenco statico di Marketo
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
source-git-commit: 68befac1804f2d6e4d42a2967577e14fef8a6ff1
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Inviare un segmento Adobe Experience Platform a un elenco statico di Marketo {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

Questa funzione ti consente di inviare in push a Marketo i segmenti situati nel Adobe Experience Platform sotto forma di un elenco statico.

>[!PREREQUISITES]
>
>* [Creare un utente API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) in Marketo.
>* Quindi, vai a **Amministratore** > **Punto di avvio**. Trova il nome del ruolo appena creato e fai clic su **Visualizza dettagli**. Copia e salva le informazioni in **ID client** e **Segreto client**, poiché ne avrai bisogno per questa funzione.


1. Accedi a [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-1.png)

1. Fai clic sull’icona della griglia e seleziona **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-2.png)

1. Nel menu di navigazione a sinistra, fai clic su **Destinazioni**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-3.png)

1. Fai clic su **Catalogo**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-4.png)

1. Trova il riquadro del Marketo Engage e fai clic su **Attiva segmenti**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-5.png)

1. Fai clic su **Configurare una nuova destinazione**.


1. In Tipo di conto, fai clic sul pulsante **Nuovo account** pulsante di scelta. Immetti le tue credenziali Marketo e fai clic su **Connetti a destinazione**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-6.png)

   >[!NOTE]
   >
   >Puoi trovare il tuo Munchkin ID andando a **Amministratore** > **Munchkin** (fa anche parte del tuo URL Marketo una volta effettuato l’accesso). ID client/Segreto è necessario seguire i prerequisiti nella parte superiore di questo articolo.

1. &quot;Connesso&quot; dovrebbe apparire sotto le tue credenziali. Fai clic su **Successivo** nell&#39;angolo in alto a destra.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-7.png)

1. Inserisci un **Nome** e _facoltativo_ Descrizione. Fai clic su **Crea destinazione**.

   >[!NOTE]
   >
   >La scelta di qualcosa dalle azioni di marketing è anche facoltativa. Marketo non utilizza tali informazioni al momento, ma probabilmente lo farà presto.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-8.png)

1. Fai clic su **Successivo**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-9.png)

1. Scegli il segmento desiderato e fai clic su **Successivo**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-10.png)

   >[!NOTE]
   >
   >Se scegli più segmenti qui, dovrai mappare ogni segmento a un elenco statico specifico nella scheda Pianificazione segmento .

1. Fai clic su **Aggiungi nuova mappatura**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-11.png)

1. Fai clic sull’icona del cursore.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-12.png)

1. Scegli la **Seleziona attributi** o **Seleziona namespace identità** pulsante di scelta (in questo esempio, stiamo scegliendo Attributi).

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-13.png)

   >[!NOTE]
   >
   >Se hai scelto **Seleziona namespace identità**, dopo aver effettuato la selezione, passa al passaggio 15.

1. Scegli il campo pertinente che contiene l’indirizzo e-mail che identifica l’utente. Fai clic su **Seleziona** al termine.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-14.png)

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-15.png)

   >[!NOTE]
   >
   >L&#39;esempio scelto può essere molto diverso dalla selezione.

1. Fai clic sull’icona di mappatura.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-16.png)

1. Scegli **Seleziona namespace identità**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-17.png)

   >[!IMPORTANT]
   >
   >Gli attributi di mappatura sono facoltativi. Mappatura di e-mail e/o ECID da **Namespace Identity** tab è la cosa più importante da fare per garantire che la persona corrisponda in Marketo. La mappatura di e-mail garantirà la percentuale di corrispondenza più elevata.

1. Scegli tra ECID o E-mail. In questo esempio scegliamo **E-mail**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-18.png)

1. Fai clic su **Successivo**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-19.png)

   >[!NOTE]
   >
   >Le identità vengono utilizzate per cercare le corrispondenze in Marketo. Se viene trovata una corrispondenza, la persona viene aggiunta all’elenco statico. Se non viene trovata una corrispondenza, queste persone vengono eliminate (ovvero, non create in Marketo).

1. _In Marketo_, crea un elenco statico oppure trova e seleziona un elenco già creato. Copia l&#39;ID di mappatura dalla fine dell&#39;URL.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-20.png)

   >[!NOTE]
   >
   >Per risultati ottimali, accertati che l’elenco a cui fai riferimento in Marketo sia vuoto.

1. In Adobe Experience Platform, immetti l&#39;ID appena copiato. Scegli la data di inizio. Le persone si sincronizzano continuamente fino alla data di fine scelta. Per una sincronizzazione indefinita, lascia vuota la data di fine. Fai clic su **Successivo** al termine.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-21.png)

1. Conferma le modifiche e fai clic su **Fine**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-22.png)
