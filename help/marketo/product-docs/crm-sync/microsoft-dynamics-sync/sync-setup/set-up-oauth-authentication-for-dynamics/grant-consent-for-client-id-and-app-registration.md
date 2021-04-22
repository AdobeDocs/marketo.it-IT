---
description: Consenso per ID client e registrazione app - Documenti Marketo - Documentazione del prodotto
title: Concessione del consenso per l’ID client e la registrazione dell’app
exl-id: d0c851d7-24a1-4b17-9daa-f0ceed39d040
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Concessione del consenso per l’ID client e la registrazione dell’app {#grant-consent-for-client-id-and-app-registration}

## Concedere le autorizzazioni dell&#39;utente delegato per l&#39;utente di sincronizzazione {#grant-delegated-user-permissions-for-the-sync-user}

1. Utilizza un programma di testo pulito (Blocco note per Windows, Modifica testo per Mac) per creare un URI (Uniform Resource Identifier) per l’autorizzazione incollando il testo seguente e sostituendo i valori client_id, redirect_uri e status.

   ```
   https://login.microsoftonline.com/common/oauth2/authorize?
   client_id='xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx'
   &response_type='code'
   &redirect_uri='https://www.<ourdomain>.com'
   &response_mode='query'
   &state='SOME_UNIQUE_UID'
   client_id value should be the client_id generated in App Registration process
   redirect_uri value should be same as value entered at the time of App registration-> Redirect URIs
   state value can be any ID (e.g.,12345)
   ```

   <table> 
    <colgroup> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>valore client_id</strong></td> 
      <td>deve essere client_id generato nel processo di registrazione dell'app</td> 
     </tr> 
     <tr> 
      <td><strong>valore redirect_uri</strong></td> 
      <td>deve essere lo stesso valore immesso al momento della registrazione dell’app &gt; URI di reindirizzamento</td> 
     </tr> 
     <tr> 
      <td><strong>valore di stato</strong></td> 
      <td>può essere qualsiasi ID (ad es. 12345)</td> 
     </tr> 
    </tbody> 
   </table>

   L’URL finale deve avere un aspetto simile al seguente: `https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. Apri l’URI creato in qualsiasi browser.

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. Accedi come utente di sincronizzazione a cui stai concedendo le autorizzazioni.

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >Se hai già effettuato l’accesso ad Azure come amministratore in un’altra scheda, dovrai utilizzare un browser o una modalità in incognito diversi per accedere come utente di sincronizzazione.

1. Fare clic su **Accetta**.

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## Concessione del consenso per tutti gli utenti {#grant-consent-for-all-users}

In qualità di amministratore, puoi anche accettare le autorizzazioni delegate di un’applicazione per conto di tutti gli utenti del tenant. Il consenso amministrativo impedisce la visualizzazione della finestra di dialogo del consenso per ogni utente nel tenant e può essere eseguito nel portale di Azure da parte degli utenti con il ruolo di amministratore. Scopri quali ruoli di amministratore possono [acconsentire alle autorizzazioni delegate qui](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference).

1. Nel portale Azure, passa alla home page dell’applicazione.

1. In Gestione, fai clic su **Autorizzazioni API**.

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. Fai clic sul pulsante **Concedi consenso amministratore** (per tenant) .

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. Fare clic su **Sì** per confermare.

   ![](assets/grant-consent-for-client-id-app-registration-6.png)

>[!MORELIKETHIS]
>
>[Configurare l’app Microsoft Dynamics CRM per On-Prem](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/set-up-microsoft-dynamics-crm-app-for-on-prem.md)
