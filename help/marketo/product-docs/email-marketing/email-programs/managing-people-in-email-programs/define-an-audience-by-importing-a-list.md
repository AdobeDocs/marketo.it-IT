---
unique-page-id: 1900597
description: Definire un pubblico importando un elenco - Documenti Marketo - Documentazione del prodotto
title: Definire un pubblico importando un elenco
exl-id: 9a63f4a5-1d76-4671-9622-19eb368d196f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 1%

---

# Definire un pubblico importando un elenco {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[Creare un messaggio e-mail per un programma e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

Dopo aver creato un programma e-mail, dovrai indicare a chi inviare l’e-mail. Puoi farlo tramite [creazione di un elenco smart](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) o importando un elenco. Ecco come eseguire questa operazione importando un elenco.

>[!NOTE]
>
>La definizione del pubblico funziona solo quando il programma e-mail non è approvato.
>
>Tutti i campi data/ora da importare vengono trattati come Ora centrale. Se si dispone di campi data/ora in un fuso orario diverso, è possibile utilizzare una formula Excel per trasformarla in Ora centrale (America/Chicago).

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Seleziona il tuo programma e-mail, quindi fai clic su Importa elenco sotto il riquadro Pubblico .

   ![](assets/importlist.png)

1. Viene visualizzata la finestra di importazione elenco, fai clic su **Sfoglia** e selezionare il file da importare. Dopo aver selezionato l&#39;elenco delle persone, fai clic su **Successivo**.

   ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >Assicurati che l’elenco sia codificato UTF-8, UTF-16, Shift-JIS o EUC-JP e non superi i 50 MB nelle dimensioni del file.

1. Verifica che i campi nel file siano mappati correttamente e fai clic su **Successivo**.

   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo ricorderà le mappature per le importazioni future.

1. Inserisci un **Nome** per l’elenco e fai clic su **Importa**.

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. Al termine dell’importazione, torna alla scheda del programma principale. Vedrete quante persone si qualificheranno.

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**Definizione**
>
>Avete notato il numero Bloccato? Questo numero è un sottoinsieme delle persone qualificate e rappresenta le persone che non possono essere inviate a questa e-mail perché sono:
>
>* Annulla l&#39;iscrizione
>* Marketing sospeso
>* Inserire nell&#39;elenco Bloccati
>* E-mail non valida
>* E-mail vuota
>
>Fare clic sul numero per un elenco dettagliato delle persone bloccate dalle spedizioni.
>
>Utilizza la ![—](assets/image2014-10-23-16-3a32-3a36-1.png) pulsante **Pubblico** per vedere quante persone si sono qualificate per ricevere l’e-mail in base ai criteri dell’elenco avanzato. Sottrai il numero Bloccato dal numero Persone per ottenere il numero totale di persone che riceveranno l’e-mail.

>[!TIP]
>
>Non è necessario attendere il completamento dell’importazione dell’elenco. Puoi continuare a lavorare se vuoi.

Fantastico! Ora è il momento di scegliere un’e-mail già esistente o di crearne una nuova da inviare a queste persone.

>[!MORELIKETHIS]
>
>* [Scegli un’e-mail esistente](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [Creare un messaggio e-mail per un programma e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

