---
description: Connettersi a Outlook - Documentazione di Marketo - Documentazione del prodotto
title: Connetti a Outlook
exl-id: 760db2d2-2e5d-4988-891a-9c57250264ac
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Connetti a Outlook {#connect-to-outlook}

Scopri come collegare l’account Sales Insight Actions a Outlook.

>[!NOTE]
>
>Ogni utente deve connettersi a Outlook dal proprio account di vendita Marketo.

## Connessione a Outlook Online {#connecting-to-outlook-online}

La connessione a Outlook ti consente di ricevere il tracciamento delle risposte, di accedere al canale di consegna di Outlook, di pianificare le e-mail in Outlook e di inviare messaggi di conformità.

1. In Marketo Sales, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/connect-to-outlook-1.png)

1. In Il mio account, seleziona **Impostazioni e-mail**.

   ![](assets/connect-to-outlook-2.png)

1. Fare clic sulla scheda **Connessione e-mail**.

   ![](assets/connect-to-outlook-3.png)

1. Fai clic su **Inizia**.

   ![](assets/connect-to-outlook-4.png)

1. Seleziona **Utilizzo Outlook per inviare e-mail** e fai clic su **Avanti**.

   ![](assets/connect-to-outlook-5.png)

1. Selezionare la versione di Outlook in uso e fare clic su **Avanti**. In questo esempio si sta scegliendo Outlook Online.

   ![](assets/connect-to-outlook-6.png)

   <table>
    <tbody>
     <tr>
      <td><strong>Outlook Online</strong></td>
      <td>Anche noto come Exchange Online</td>
     </tr>
     <tr>
      <td><strong>Exchange On-Premise</strong></td>
      <td>Include Exchange 2013 e 2016</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Al momento, Marketo non supporta gli account ibridi di Exchange.

1. Fai clic su **OK**.

   ![](assets/connect-to-outlook-7.png)

1. Se non hai effettuato l&#39;accesso a Outlook, immetti le tue informazioni di accesso e fai clic su **Avanti**. In caso affermativo, scegliere l&#39;account a cui connettersi e fare clic su **Avanti**. In questo esempio, abbiamo già effettuato l’accesso.

   ![](assets/connect-to-outlook-8.png)

1. Fare clic su **Accetta**.

   ![](assets/connect-to-outlook-9.png)

   Puoi utilizzare questa connessione per tenere traccia delle e-mail e anche come canale di consegna.

   >[!NOTE]
   >
   >Outlook Online (Office365) applica i propri limiti di invio. [Ulteriori informazioni](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md#email-provider-limits).

## Connessione a Exchange On-Premise {#connecting-to-exchange-on-premise}

La connessione a Exchange On-Premise ti consente di ricevere il tracciamento delle risposte, di accedere al canale di consegna di Outlook, di pianificare le e-mail in Outlook e di inviare messaggi di conformità.

1. In Marketo Sales, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/connect-to-outlook-10.png)

1. In Il mio account, seleziona **Impostazioni e-mail**.

   ![](assets/connect-to-outlook-11.png)

1. Fare clic sulla scheda **Connessione e-mail**.

   ![](assets/connect-to-outlook-12.png)

1. Fai clic su **Inizia**.

   ![](assets/connect-to-outlook-13.png)

1. Seleziona **Utilizzo Outlook per inviare e-mail** e fai clic su **Avanti**.

   ![](assets/connect-to-outlook-14.png)

1. Selezionare la versione di Outlook in uso e fare clic su **Avanti**. In questo esempio viene scelto Exchange On-Premise.

   ![](assets/connect-to-outlook-15.png)

   <table>
    <tbody>
     <tr>
      <td><strong>Outlook Online</strong></td>
      <td>Anche noto come Exchange Online</td>
     </tr>
     <tr>
      <td><strong>Exchange On-Premise</strong></td>
      <td>Include Exchange 2013 e 2016</td>
     </tr>
    </tbody>
   </table>

1. Immetti le credenziali e fai clic su **Connetti**.

   ![](assets/connect-to-outlook-16.png)

   >[!NOTE]
   >
   >Se si disattiva l&#39;individuazione automatica nel menu a discesa Versione di Exchange, sarà necessario chiedere al reparto IT l&#39;URL di Exchange.

   Puoi utilizzare questa connessione per tenere traccia delle e-mail e anche come canale di consegna.

   >[!NOTE]
   >
   >Quando utilizzi Exchange On-Prem, il team IT stabilirà il limite di invio delle e-mail.

## Ottenimento delle autorizzazioni per la connessione a Outlook Online {#getting-permission-to-connect-to-outlook-online}

È possibile che sia necessario collaborare con il team IT per ottenere l&#39;autorizzazione per consentire a Marketo Sales di connettersi all&#39;account Outlook Online (Microsoft 365).

>[!NOTE]
>
>Informare il team IT che gestisce l&#39;account Microsoft 365 che l&#39;applicazione a cui è necessario accedere è &quot;Marketo Sales Connect&quot;.

A seconda delle preferenze del team IT e della configurazione corrente, è consigliabile consultare il team IT per informazioni su come concedere l&#39;accesso. Di seguito sono riportati alcuni articoli che possono contribuire a guidare la conversazione.

* Consenso globale: [App integrate e Azure AD per amministratori di Microsoft 365](https://learn.microsoft.com/en-us/microsoft-365/enterprise/integrated-apps-and-azure-ads?view=o365-worldwide){target="_blank"}
* Consenso utente: [Configura il consenso degli utenti alle applicazioni](https://learn.microsoft.com/en-us/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal&pivots=portal){target="_blank"}
* Consenso amministratore: [Configura il flusso di lavoro del consenso amministratore](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&view=o365-worldwide){target="_blank"}
* Attivazione o disattivazione del consenso utente: [Gestione del consenso degli utenti alle app in Microsoft 365](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&view=o365-worldwide){target="_blank"}
* Gestione con Microsoft Defender: [Gestione app OAuth](https://learn.microsoft.com/en-us/defender-cloud-apps/manage-app-permissions){target="_blank"}
