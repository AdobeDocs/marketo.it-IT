---
unique-page-id: 2949711
description: Installa il componente aggiuntivo Marketo Email per  [!DNL Outlook]  con un codice di registrazione - Documentazione di Marketo - Documentazione del prodotto
title: Installa Marketo Email Add-in per  [!DNL Outlook]  con un codice di registrazione
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 4%

---

# Installare il componente aggiuntivo e-mail di Marketo per [!DNL Outlook] con un codice di registrazione {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

Se gli utenti possono accedere alle impostazioni di amministrazione sui propri laptop, puoi inviare loro direttamente un codice di registrazione.

Se non hai ricevuto un’e-mail di invito, chiedi all’amministratore di Marketo di invitarti.

>[!PREREQUISITES]
>
>È necessario [emettere una licenza di Marketo Email Add-in](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md).

>[!IMPORTANT]
>
>L&#39;installazione non è supportata nei PC in cui la cartella dell&#39;utente di Windows contiene caratteri non inglesi. Questa cartella viene generata automaticamente da Windows in `<System Root>\Users\` in base al nome utente di Windows e può contenere caratteri non inglesi se il nome utente di Windows è un nome non inglese. Collabora con il tuo team IT per verificare se stai riscontrando problemi di installazione.

>[!NOTE]
>
>Le funzionalità delle azioni di Sales Insight, tra cui Invia e-mail per le vendite, Aggiungi a campagna vendite e Attività, non sono disponibili nei plug-in e-mail di Sales Insight per Gmail e Outlook. Al momento, gli utenti possono inviare un’e-mail tracciabile solo con o senza un modello e-mail di Marketo dal proprio client e-mail quando utilizzano i plug-in e-mail di Sales Insight.

## Scarica programma di installazione {#download-installer}

1. Identificare la [versione di Microsoft Outlook](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c){target="_blank"}.

1. Nella tabella seguente, fare clic sul collegamento per scaricare il file .ZIP appropriato per la versione di Microsoft Outlook in uso.

1. Decomprimi il file per accedere al file .MSI necessario e procedi con l’installazione.

   >[!NOTE]
   >
   >Al momento, i collegamenti seguenti funzionano solo in [!DNL Microsoft Edge] o facendo clic con il pulsante destro del mouse in [!DNL Chrome]. Ci scusiamo per l&#39;inconveniente.

<table><thead>
  <tr>
    <th>Versione di Outlook</th>
    <th>Outlook a 32 bit</th>
    <th>Outlook a 64 bit</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Outlook 2000</td>
    <td>Non supportato</td>
    <td>N/D</td>
  </tr>
  <tr>
    <td>Outlook 2003</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Scarica</a></td>
    <td>N/D</td>
  </tr>
  <tr>
    <td>Outlook 2007</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Scarica</a></td>
    <td>N/D</td>
  </tr>
  <tr>
    <td>Outlook 2010</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Scarica</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Scarica</a></td>
  </tr>
  <tr>
    <td>Outlook 2013</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Scarica</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Scarica</a></td>
  </tr>
  <tr>
    <td>Outlook 2016</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Scarica</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Scarica</a></td>
  </tr>
  <tr>
    <td>Outlook 2019</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Scarica</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Scarica</a></td>
  </tr>
  <tr>
    <td>Outlook per Mac</td>
    <td>Non supportato</td>
    <td>Non supportato</td>
  </tr>
  <tr>
    <td>Outlook Web App</td>
    <td>Non supportato</td>
    <td>Non supportato</td>
  </tr>
  <tr>
    <td>Office 365*</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Scarica</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Scarica</a></td>
  </tr>
</tbody></table>

*[!DNL Office] versione 365: solo client [!DNL Windows] (su [!DNL Windows] 10, [!DNL Enterprise] o [!DNL Pro]).

>[!IMPORTANT]
>
>Microsoft ha rilasciato una [nuova versione di Outlook per Windows](https://techcommunity.microsoft.com/t5/outlook-blog/new-outlook-for-windows-now-available/ba-p/3932068){target="_blank"}. Questa nuova versione non supporta il plug-in di Outlook MSI esistente. Il plug-in MSI Outlook continuerà a funzionare per i desktop Windows che eseguono la versione classica di Outlook. Per ulteriori informazioni sul nuovo Outlook per Windows per le organizzazioni, [fare clic qui](https://techcommunity.microsoft.com/t5/outlook-blog/the-new-outlook-for-windows-for-organization-admins/ba-p/3929169){target="_blank"}.

## Copia il codice di registrazione {#copy-your-registration-code}

1. Copia il codice di registrazione dall’e-mail di invito ricevuta.

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. Chiudi [!DNL Microsoft Outlook].

   ![](assets/ent-key-close-outlook-hand.png)

## Installa {#install}

1. Eseguire il programma di installazione.

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >Se ricevi un avviso di sicurezza, non preoccuparti! Fai clic su **Esegui**.

1. Fai clic su **[!UICONTROL Next]**.

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. Compila **[!UICONTROL First Name]**, **[!UICONTROL Last Name]**, **[!UICONTROL Email Address]**, quindi copia e incolla **[!UICONTROL Registration code]** dall&#39;e-mail nel modulo e fai clic su **[!UICONTROL Next]**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >Se l&#39;installazione non riesce, rivolgiti al reparto IT per verificare che il traffico HTTPS non sia bloccato. Il programma di installazione richiede l&#39;apertura del traffico HTTPS.

1. Fare clic su **[!UICONTROL Next]** per installare nel percorso predefinito.

   ![](assets/select-installation-folder-hand.png)

1. Fai clic su **[!UICONTROL Next]**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >Se viene visualizzato un messaggio di sicurezza relativo a un autore sconosciuto, fare clic su **[!UICONTROL Yes]**.

1. Installazione completata. Fare clic su **[!UICONTROL Close]**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Aprire [!DNL Microsoft Outlook] e visualizzare i pulsanti di Marketo.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   Eccellente! I pulsanti Marketo sono ora posizionati in modo migliore.

Ulteriori informazioni sull&#39;utilizzo delle azioni Messaggio di Marketo e Registra con Marketo.

>[!MORELIKETHIS]
>
>* [Inviare e tenere traccia di un&#39;e-mail con il componente aggiuntivo e-mail di Marketo per Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md){target="_blank"}
>* [Invia e tieni traccia di Outlook utilizzando un modello di Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md){target="_blank"}
