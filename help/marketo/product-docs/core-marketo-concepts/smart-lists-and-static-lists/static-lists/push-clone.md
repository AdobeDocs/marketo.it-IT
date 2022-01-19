---
description: Clone push - Documenti Marketo - Documentazione del prodotto
title: Clona push
hide: true
hidefromtoc: true
source-git-commit: 8920bc525075923b32e7330da20debb7b8f47b06
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Clona push {#push-clone}

Questa funzione ti consente di inviare in push a Marketo i segmenti situati nel Adobe Experience Platform sotto forma di un elenco statico.

>[!PREREQUISITES]
>
>* [Creare un utente API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) in Marketo.
>* Quindi, vai a **Amministratore** > **Punto di avvio**. Trova il nome del ruolo appena creato e fai clic su **Visualizza dettagli**. Copia e salva le informazioni in **ID client** e **Segreto client**, poiché ne avrai bisogno per questa funzione.


1. Accedi a [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. Fai clic sull’icona della griglia e seleziona **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. Nel menu di navigazione a sinistra, fai clic su **Destinazioni**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. Fai clic su **Catalogo**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. Trova il riquadro del Marketo Engage e fai clic su **Attiva segmenti**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. Fai clic su **Configurare una nuova destinazione**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. In Tipo di conto selezionare il pulsante di opzione Esistente o Nuovo account (in questo esempio, stiamo scegliendo **Account esistente**). Fai clic sull’icona Seleziona account .

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

1. Scegli l’account di destinazione e fai clic su **Seleziona**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

Ora dovrai scegliere se desideri far corrispondere solo le persone Marketo esistenti, o far corrispondere le persone Marketo esistenti e creare le persone mancanti in Marketo. Di seguito sono riportate le sezioni che descrivono come eseguire ciascuna operazione.

## Corrispondenza con le persone esistenti di Marketo e creazione di persone mancanti in Marketo {#match-existing-marketo-people-create-missing-people}

Dopo aver seguito i passaggi 1-8 dall&#39;alto...

1. Immettere una destinazione **Nome** e una descrizione facoltativa. Fare clic sull&#39;elenco a discesa Creazione persona e selezionare **Corrispondenza con le persone esistenti di Marketo e creazione di persone mancanti in Marketo**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

1. Questa sezione è facoltativa. Fai clic su **Crea** per saltare.

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. Seleziona la destinazione creata e fai clic su **Successivo**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. Scegli il segmento da inviare a Marketo e fai clic su **Successivo**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

1. Fai clic su **Aggiungi nuova mappatura**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. Fai clic sull’icona di mappatura.

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. Mappa nome selezionando **firstName** e facendo clic su **Seleziona**.

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

1. Mappa il cognome e il nome della società facendo clic su **Aggiungi nuova mappatura** di nuovo e ripetendo il passaggio 7 due volte, scegliendo lastName e quindi companyName.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. Ora è il momento di mappare l’indirizzo e-mail. Fai clic su **Aggiungi nuova mappatura** di nuovo.

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. Fai clic sull’icona di mappatura.

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. Fai clic sul pulsante di opzione Seleziona namespace identità , scegli  **E-mail**, quindi fai clic su **Seleziona**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

1. Ora è il momento di scegliere i campi di origine. Per e-mail, fai clic sull’icona del cursore.

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. Fai clic sul pulsante di opzione Seleziona namespace identità , trova e seleziona **E-mail**, quindi fai clic su **Seleziona**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

MORREEE

## Solo persone Marketo esistenti {#match-existing-marketo-people-only}

>[!NOTE]
>
>Le identità vengono utilizzate per cercare le corrispondenze in Marketo. Se viene trovata una corrispondenza, la persona viene aggiunta all’elenco statico. Se non viene trovata una corrispondenza, queste persone vengono eliminate (ovvero, non create in Marketo).

1. _In Marketo_, crea un elenco statico oppure trova e seleziona un elenco già creato. Copia l&#39;ID di mappatura dalla fine dell&#39;URL.

PICC

>[!NOTE]
>
>Per risultati ottimali, accertati che l’elenco a cui fai riferimento in Marketo sia vuoto.

1. In Adobe Experience Platform, immetti l&#39;ID appena copiato. Scegli la data di inizio. Le persone si sincronizzano continuamente fino alla data di fine scelta. Per una sincronizzazione indefinita, lascia vuota la data di fine. Fai clic su **Successivo** al termine.

PICC

1. Conferma le modifiche e fai clic su **Fine**.

PICC
