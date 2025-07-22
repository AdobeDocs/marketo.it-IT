---
unique-page-id: 14352484
description: Come risolvere il problema "Impossibile autenticare la richiesta" durante la connessione a Salesforce - Documentazione di Marketo - Documentazione del prodotto
title: Come risolvere il problema "Impossibile autenticare la richiesta" durante la connessione a Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 3%

---

# Come correggere &quot;Impossibile autenticare la richiesta&quot; durante la connessione a [!DNL Salesforce] {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Se durante il tentativo di connessione di [!DNL Sales Connect] a [!DNL Salesforce] viene visualizzato il messaggio di errore &quot;Impossibile autenticare la richiesta&quot;, è possibile che l&#39;accesso all&#39;API di [!DNL Salesforce] sia limitato. Rivolgiti all&#39;amministratore di [!DNL Salesforce] per verificare che siano presenti i seguenti elementi.

## Abilitare l’API nelle autorizzazioni utente {#enable-api-in-user-permissions}

1. Richiedi a un amministratore [!DNL Salesforce] di accedere a SFDC.
1. Seleziona **[!UICONTROL Setup]**.
1. Seleziona **[!UICONTROL Manage Users]**.
1. Seleziona **[!UICONTROL Profiles]**.
1. Trovare il profilo in cui si trovano gli utenti ToutApp e fare clic su **[!UICONTROL Edit]**.
1. Scorri verso il basso fino a **[!UICONTROL Administrative Permissions]** e accertati che **[!UICONTROL API Enabled]** sia selezionato.

## Controlla se [!DNL Salesforce] sta bloccando la connessione a [!DNL Sales Connect] {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Chiedi a un amministratore di [!DNL Salesforce] di accedere a SFDC.
1. Seleziona **[!UICONTROL Setup]**.
1. Seleziona **[!UICONTROL Manage Apps]**.
1. Seleziona **[!UICONTROL Connected Apps OAuth Usage]**.
1. Assicurarsi che [!DNL Sales Connect] sia affiancato da &quot;[!UICONTROL Block]&quot;. Se vedi &quot;[!UICONTROL Unblock]&quot;, fai clic sul pulsante per sbloccare l&#39;accesso di [!DNL Sales Connect] a [!DNL Salesforce].
