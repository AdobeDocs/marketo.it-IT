---
unique-page-id: 2360356
description: Aggiunta del Single Sign-On a un portale - Documentazione Marketo - Documentazione del prodotto
title: Aggiungere il Single Sign-On a un portale
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
feature: Administration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Aggiungere il Single Sign-On a un portale {#add-single-sign-on-to-a-portal}

Se si dispone di un servizio directory che autentica gli utenti, è possibile consentire l&#39;accesso Single Sign-On (SSO) in Marketo. Questa funzionalità è supportata con [!DNL Security Assertion Markup Language] (SAML) versione 2.0 e successive.

Marketo funziona come provider di servizi SAML (SP) e dipende da un provider di identità esterno (IdP) per l’autenticazione degli utenti.

Una volta abilitato l&#39;SSO, l&#39;IdP può convalidare le credenziali di un utente. Quando un utente desidera utilizzare il software Marketo, l&#39;IdP invia un messaggio SAML firmato a Marketo, che funge da SP. Questo messaggio garantisce a Marketo che l&#39;utente è autorizzato a utilizzare il software Marketo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!IMPORTANT]
>
>Questo non si applica agli abbonamenti a cui è stato effettuato l’onboarding in Adobe Identity. Per gli abbonamenti a cui è stato effettuato l’onboarding in Adobe Identity, l’accesso Single Sign-On è configurato a livello di organizzazione Adobe in Adobe Admin Console. Al momento, Adobe Admin Console supporta solo gli SP avviati. [Ulteriori informazioni](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>Sei un utente di [!DNL Microsoft Azure]? Consulta la loro [esercitazione sull&#39;integrazione](https://learn.microsoft.com/en-us/entra/identity/saas-apps/marketo-tutorial){target="_blank"}. Per informazione, nel passaggio 5c dell’esercitazione è presente un errore di battitura. Impostare lo stato di inoltro su `https://<munchkinid>.mktoweb.com`, **_not_** `https://<munchkinid>.marketo.com`.

## Come inviare la richiesta {#how-to-send-the-request}

* Invia la richiesta SSO, che è una risposta SAML, a `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Come URL del pubblico dell’SP. Usa `http://saml.marketo.com/sp`
* Se si utilizza l&#39;attributo SPNameQualifier, impostare l&#39;elemento NameID per Subject su `http://saml.marketo.com/sp`
* Se si stanno federando più sottoscrizioni Marketo allo stesso provider SSO, è possibile utilizzare URL SP univoci per ogni sottomissione Marketo con il formato `http://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo supporta solo le pagine avviate dal provider di identità (note anche come avviate da IdP), in cui l’utente avvia per la prima volta la pagina di accesso IdP, si autentica e poi passa a Il mio Marketo. Se la sottoscrizione a Marketo è stata spostata in Admin Console, al momento Adobe Admin Console supporta solo le sottoscrizioni avviate dal provider di servizi (note anche come avviate da SP). Potrebbero essere state apportate modifiche nell&#39;esperienza SSO.

## Note aggiuntive {#additional-notes}

* **Tempo di sincronizzazione** - Per un nuovo utente, trascorrono circa 10 minuti prima che venga elaborata una richiesta SSO iniziale.
* **Provisioning utenti** - Gli utenti dispongono del provisioning manuale tramite Marketo.
* **Autorizzazione** - Le autorizzazioni utente vengono mantenute in Marketo.
* **Supporto OAuth** - Marketo non supporta attualmente OAuth.
* **Propagazione utente automatica** - Nota anche come &quot;Just in Time Provisioning&quot;, si verifica quando il primo accesso SAML di un utente è in grado di creare l&#39;utente in qualsiasi applicazione Web a cui sta accedendo (ad esempio, Marketo) e non è richiesta alcuna azione manuale da parte dell&#39;amministratore. Al momento questo non è supportato da Marketo.
* **Crittografia** - Marketo non supporta attualmente la crittografia.

>[!NOTE]
>
>Prima di iniziare, assicurati di disporre del certificato del provider di identità in formato X.509 e dell’estensione .crt, .der o .cer.

## Aggiorna impostazioni SAML {#update-saml-settings}

SSO è disabilitato per impostazione predefinita. Per abilitare SAML e configurarlo, segui la procedura riportata di seguito.

1. Passare all&#39;area **[!UICONTROL Admin]**.

   ![](assets/add-single-sign-on-to-a-portal-1.png)

1. Fai clic su **[!UICONTROL Single Sign-On]**.

   ![](assets/add-single-sign-on-to-a-portal-2.png)

   >[!NOTE]
   >
   >Se non vedi **[!UICONTROL Single Sign-On]** in **[!UICONTROL Admin]**, contatta il [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. Nella sezione **[!UICONTROL SAML Settings]** fare clic su **[!UICONTROL Edit]**.

   ![](assets/add-single-sign-on-to-a-portal-3.png)

1. Cambia **[!UICONTROL SAML Single Sign-On]** in **[!UICONTROL Enabled]**.

   ![](assets/add-single-sign-on-to-a-portal-4.png)

1. Immetti **[!UICONTROL Issuer ID]**, **[!UICONTROL Entity ID]**, seleziona **[!UICONTROL User ID Location]**, quindi fai clic su **[!UICONTROL Browse]**.

   ![](assets/add-single-sign-on-to-a-portal-5.png)

1. Selezionare il file **[!UICONTROL Identity Provider Certificate]**.

   ![](assets/add-single-sign-on-to-a-portal-6.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/add-single-sign-on-to-a-portal-7.png)

## Aggiorna impostazioni pagina di reindirizzamento {#update-redirect-page-settings}

1. Nella sezione **[!UICONTROL Redirect Pages]** fare clic su **[!UICONTROL Edit]**.

   ![](assets/add-single-sign-on-to-a-portal-8.png)

   >[!NOTE]
   >
   >I clienti che utilizzano Universal ID insieme all&#39;SSO devono immettere l&#39;URL di accesso del provider di identità nel campo **[!UICONTROL Login URL]**.

1. Immetti **[!UICONTROL Logout URL]**. Questo è l’URL a cui desideri che l’utente venga indirizzato quando esce da Marketo.

   ![](assets/add-single-sign-on-to-a-portal-9.png)

1. Immetti un **[!UICONTROL Error URL]**. Questo è l’URL a cui desideri indirizzare l’utente nel caso in cui l’accesso a Marketo non riesca. Fai clic su **[!UICONTROL Save]**.

   ![](assets/add-single-sign-on-to-a-portal-10.png)

   >[!NOTE]
   >
   >Entrambe queste pagine devono essere pubbliche.

>[!MORELIKETHIS]
>
>* [Utilizzo di un ID universale per l&#39;accesso all&#39;abbonamento](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md){target="_blank"}
>* [Limita l&#39;accesso utente solo a SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target="_blank"}
>* [Invito di utenti Marketo a due istanze con ID universale](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target="_blank"}
