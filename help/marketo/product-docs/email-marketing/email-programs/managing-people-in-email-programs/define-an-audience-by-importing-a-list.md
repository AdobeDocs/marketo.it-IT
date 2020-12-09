---
unique-page-id: 1900597
description: Definire un pubblico importando un elenco - Documenti Marketo - Documentazione prodotto
title: Definire un pubblico importando un elenco
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# Definire un pubblico importando un elenco {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[Creare un&#39;e-mail per un programma e-mail](../../../../product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

Dopo aver creato un programma e-mail, è necessario indicare a chi inviare l&#39;e-mail. È possibile eseguire questa operazione [creando un elenco](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) avanzato o importando un elenco. Questo è il modo per farlo importando un elenco.

>[!NOTE]
>
>La definizione del pubblico funzionerà solo se il programma e-mail non è approvato.
>
>Tutti i campi data/ora importati vengono considerati come Ora centrale. Se i campi data/ora si trovano in un fuso orario diverso, è possibile utilizzare una formula Excel per trasformarla in Ora centrale (America/Chicago).

1. Vai a Attività **** di marketing.

   ![](assets/login-marketing-activities-1.png)

   Selezionate il programma e-mail e fate clic su Importa elenco sotto la sezione Pubblico.
   ![](assets/importlist.png)

1. Viene visualizzata la finestra di importazione dell’elenco, fate clic su **Sfoglia** e selezionate il file da importare. Dopo aver selezionato l’elenco delle persone, fate clic su Avanti.
1. ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >Verificate che l&#39;elenco sia codificato UTF-8, UTF-16, Shift-JIS o EUC-JP e che le dimensioni del file non superino i 50 MB.

   Verificate che i campi nel file siano mappati correttamente e fate clic su Avanti.
   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo ricorderà le mappature per le importazioni future!

1. Immettete un **nome** per l’elenco e fate clic su **Importa**.

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. Al termine dell&#39;importazione, tornare alla scheda principale del programma. Vedrai quante persone si qualificheranno.

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**Definizione**
>
>Avete notato il numero Bloccato? Questo numero è un sottoinsieme di persone qualificate e rappresenta le persone che non possono essere inviate a questo messaggio perché sono:
>
>* Annulla sottoscrizione
>* Marketing sospeso
>*  Inserire nell&#39;elenco Bloccati
>* E-mail non valida
>* E-mail vuota

>
>
Fare clic sul numero per un elenco dettagliato di persone bloccate dalle spedizioni.
>
>Utilizzate il pulsante ![—](assets/image2014-10-23-16-3a32-3a36-1.png) nella sezione **Pubblico** per vedere quante persone sono qualificate per ricevere l&#39;e-mail in base ai criteri dell&#39;elenco avanzato. Sottrai il numero Bloccato dal numero Persone per ottenere il numero totale di persone che riceveranno l’e-mail.

>[!TIP]
>
>Non è necessario attendere il termine dell&#39;importazione dell&#39;elenco. Puoi continuare a lavorare se vuoi.

Fantastico! Ora è il momento di scegliere un&#39;e-mail già esistente o di creare una nuova e-mail da inviare a queste persone.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Scegliere un&#39;e-mail esistente](../../../../product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [Creare un&#39;e-mail per un programma e-mail](../../../../product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

>



