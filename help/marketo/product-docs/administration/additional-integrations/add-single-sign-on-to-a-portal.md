---
unique-page-id: 2360356
description: Aggiungere Single Sign-On a un portale - Documenti Marketo - Documentazione del prodotto
title: Aggiungere Single Sign-On a un portale
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---


# Aggiungi Single Sign-On a un portale {#add-single-sign-on-to-a-portal}

Se disponi di un servizio di directory che autentica gli utenti, puoi consentire l’accesso single sign-on (SSO) in Marketo. Supportiamo questa funzione utilizzando la versione 2.0 o successiva di Security Assertion Markup Language (SAML).

Marketo funziona come provider di servizi SAML (SP) e dipende da un provider di identità esterno (IdP) per l’autenticazione degli utenti.

Una volta abilitato l’SSO, l’IdP può convalidare le credenziali di un utente. Quando un utente desidera utilizzare il software Marketo, l&#39;IdP invia quindi un messaggio SAML firmato a Marketo, agendo come SP. Questo messaggio garantisce a Marketo che l&#39;utente è autorizzato a utilizzare il software Marketo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>Sei un utente di Microsoft Azure? Consulta la relativa [esercitazione sull&#39;integrazione](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/).

## Come inviare la richiesta {#how-to-send-the-request}

* Invia la richiesta SSO, che è una risposta SAML, a `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Come URL del pubblico dell’SP. Usa `https://saml.marketo.com/sp`
* Se utilizzi l’attributo SPNameQualifier, imposta l’elemento NameID per Subject su `https://saml.marketo.com/sp`
* Se federi più abbonamenti Marketo allo stesso provider SSO, puoi utilizzare URL SP univoci per ogni sottomodulo Marketo con il formato `https://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo supporta solo il provider di identità (noto anche come IdP-started), in cui l’utente avvia per la prima volta la pagina di accesso Idp, si autentica, quindi passa a My Marketo.

## Note aggiuntive {#additional-notes}

* **Tempo**  di sincronizzazione: per un nuovo utente, si verifica circa 10 minuti di ritardo prima dell&#39;elaborazione di una richiesta SSO iniziale.
* **Provisioning utente** : il provisioning degli utenti viene eseguito manualmente da Marketo.
* **Autorizzazione** : le autorizzazioni utente vengono mantenute in Marketo.
* **Supporto OAuth** : Marketo al momento non supporta OAuth.
* **Propagazione automatica degli utenti** : nota anche come &quot;Just in Time Provisioning&quot; (Provisioning in tempo), quando il primo accesso SAML di un utente è in grado di creare l&#39;utente in qualsiasi applicazione Web a cui accede (ad esempio, Marketo) e non è necessaria alcuna azione manuale di amministrazione. Al momento Marketo non supporta questa funzionalità.
* **Crittografia** : Marketo al momento non supporta la crittografia.

>[!NOTE]
>
>Prima di iniziare, chiedi al certificato del provider di identità in formato X.509 e con estensione crt, der o cer.

## Aggiorna le impostazioni SAML {#update-saml-settings}

SSO è disattivato per impostazione predefinita. Segui questi passaggi per abilitare SAML e configurarlo.

1. Vai su **Amministratore** e fai clic su **Single Sign-On**.

   ![](assets/image2014-9-24-14-3a36-3a50.png)

   >[!NOTE]
   >
   >Se non trovi **Single Sign-On** in **Amministratore**, contatta il [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Nella sezione **Impostazioni SAML**, fai clic su **Modifica**.

   ![](assets/image2014-9-24-14-3a37-3a3.png)

1. Cambia **Single Sign-On SAML** in **Abilitato**.

   ![](assets/image2014-9-24-14-3a37-3a17.png)

1. Immetti il tuo **ID emittente**, **ID entità**, seleziona la **Posizione ID utente**, quindi fai clic su **Sfoglia**.

   ![](assets/image2014-9-24-14-3a37-3a32.png)

1. Seleziona il file **Certificato del fornitore di identità**.

   ![](assets/image2014-9-24-14-3a38-3a8.png)

1. Fare clic su **Salva**.

   ![](assets/image2014-9-24-14-3a38-3a22.png)

## Aggiorna impostazioni pagina di reindirizzamento {#update-redirect-page-settings}

1. Nella sezione **Pagine di reindirizzamento**, fai clic su **Modifica**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >I clienti che utilizzano l’ID universale insieme all’SSO devono immettere l’URL di accesso del provider di identità nel campo **URL di accesso** .

1. Immetti un **URL di disconnessione**. Questo è l’URL a cui si desidera indirizzare l’utente quando si disconnette da Marketo.

   ![](assets/eight.png)

1. Immetti un **URL di errore**. Questo è l’URL a cui si desidera indirizzare l’utente nel caso in cui l’accesso a Marketo non riesca. Fare clic su **Salva**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Entrambe le pagine devono essere accessibili al pubblico.

>[!MORELIKETHIS]
>
>* [Utilizzo di un ID universale per l’accesso all’abbonamento](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Limita accesso utente solo a SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [Invitare gli utenti di Marketo a due istanze con ID universale](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

