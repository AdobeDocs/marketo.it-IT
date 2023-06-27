---
unique-page-id: 2949711
description: Installare Marketo Email Add-in per Outlook con un codice di registrazione - Documentazione di Marketo - Documentazione del prodotto
title: Installare Marketo Email Add-in per Outlook con un codice di registrazione
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
source-git-commit: 8b9b2b83f5dc8908f9794d1ee387299edaae31b3
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 3%

---

# Installare Marketo Email Add-in per Outlook con un codice di registrazione {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

Se gli utenti possono accedere alle impostazioni di amministrazione sui propri laptop, puoi inviare loro direttamente un codice di registrazione.

Se non hai ricevuto un’e-mail di invito, chiedi all’amministratore di Marketo di invitarti.

>[!PREREQUISITES]
>
>Devi essere [ha emesso una licenza di Marketo Email Add-in](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md).

>[!IMPORTANT]
>
>L&#39;installazione non è supportata nei PC in cui la cartella dell&#39;utente di Windows contiene caratteri non inglesi. Questa cartella viene generata automaticamente da Windows in `<System Root>\Users\` in base al nome utente di Windows e può contenere caratteri non inglesi se il nome utente di Windows è un nome non inglese. Collabora con il tuo team IT per verificare se stai riscontrando problemi di installazione.

>[!NOTE]
>
>Le funzionalità delle azioni di approfondimento delle vendite, tra cui Invia e-mail alle vendite, Aggiungi a campagna di vendita e Attività, non sono disponibili nei plug-in e-mail di approfondimento delle vendite per Gmail e Outlook. Al momento, gli utenti possono inviare un’e-mail tracciabile solo con o senza un modello e-mail di Marketo dal proprio client e-mail quando utilizzano i plug-in e-mail di Sales Insight.

## Scarica programma di installazione {#download-installer}

1. Identificare [Versione di Microsoft Outlook](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c){target="_blank"}

1. Fare clic sul collegamento per scaricare il programma di installazione appropriato per la versione di Microsoft Outlook in uso.

   >[!NOTE]
   >
   >Al momento, i collegamenti riportati di seguito funzionano solo in Microsoft Edge o facendo clic con il pulsante destro del mouse in Chrome. Ci scusiamo per l&#39;inconveniente.

   | Versione di Outlook | Outlook a 32 bit | Outlook a 64 bit |
   |---|---|---|
   | Outlook 2000 | Non supportato | N/D |
   | Outlook 2003 | [Scarica](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | N/D |
   | Outlook 2007 | [Scarica](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | N/D |
   | Outlook 2010 | [Scarica](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Scarica](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2013 | [Scarica](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Scarica](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2016 | [Scarica](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Scarica](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2019 | [Scarica](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Scarica](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook per Mac | Non supportato | Non supportato |
   | Outlook Web App | Non supportato | Non supportato |
   | Office 365* | [Scarica](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Scarica](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |

   *Versione Office 365: solo client Windows (su Windows 10, Enterprise o Pro).

## Copia il codice di registrazione {#copy-your-registration-code}

1. Copia il codice di registrazione dall’e-mail di invito ricevuta.

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. Chiudere Microsoft Outlook.

   ![](assets/ent-key-close-outlook-hand.png)

## Installa {#install}

1. Eseguire il programma di installazione.

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >Se ricevi un avviso di sicurezza, non preoccuparti! Fai clic su **Esegui**.

1. Clic **Successivo**.

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. Compila **Nome**, **Cognome**, **Indirizzo e-mail**, quindi copia e incolla il **Codice di registrazione** dall’e-mail al modulo e fai clic su **Successivo**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >Se l&#39;installazione non riesce, rivolgiti al reparto IT per verificare che il traffico HTTPS non sia bloccato. Il programma di installazione richiede l&#39;apertura del traffico HTTPS.

1. Clic **Successivo** per eseguire l&#39;installazione nel percorso predefinito.

   ![](assets/select-installation-folder-hand.png)

1. Clic **Successivo**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >Se ricevi una richiesta di sicurezza relativa a un editore sconosciuto, fai clic su **Sì**.

1. L&#39;installazione è stata completata, fare clic su **Chiudi**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Aprire Microsoft Outlook e visualizzare i pulsanti di Marketo.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   Eccellente! I pulsanti Marketo sono ora posizionati in modo migliore.

Ulteriori informazioni sull&#39;utilizzo delle azioni Messaggio di Marketo e Registra con Marketo.

>[!MORELIKETHIS]
>
>* [Inviare e tenere traccia di un messaggio e-mail con il componente aggiuntivo e-mail di Marketo per Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md){target="_blank"}
>* [Inviare e tenere traccia di Outlook utilizzando un modello di Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md){target="_blank"}
