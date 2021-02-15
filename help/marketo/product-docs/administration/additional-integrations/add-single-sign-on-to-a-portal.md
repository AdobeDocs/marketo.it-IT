---
unique-page-id: 2360356
description: Aggiunta di Single Sign-On a un portale - Documenti Marketo - Documentazione prodotto
title: Aggiunta di Single Sign-On a un portale
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# Aggiunta di Single Sign-On a un portale {#add-single-sign-on-to-a-portal}

Se disponete di un servizio di directory che esegue l&#39;autenticazione degli utenti, potete consentire l&#39;accesso singolo (SSO) a Marketo. Supportiamo questa funzione utilizzando il linguaggio SAML (Security Assertion Markup Language) versione 2.0 e successive.

Marketo funziona come provider di servizi SAML (SP) e dipende da un provider di identità (IdP) esterno per l&#39;autenticazione degli utenti.

Una volta attivato SSO, l&#39;IdP può convalidare le credenziali di un utente. Quando un utente desidera utilizzare il software Marketo, l&#39;IdP invia quindi un messaggio SAML firmato a Marketo, in qualità di SP. Questo messaggio garantisce a Marketo che l&#39;utente è autorizzato a utilizzare il software Marketo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>Sei un utente di Microsoft Azure? Controlla la loro [esercitazione sull&#39;integrazione](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/).

## Come inviare la richiesta {#how-to-send-the-request}

* Invia la richiesta SSO, che è una risposta SAML, a `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Come URL pubblico dell&#39;SP. Utilizzare [https://saml.marketo.com/sp](https://saml.marketo.com/sp)
* Se utilizzate l&#39;attributo SPNameQualifier, impostate l&#39;elemento NameID per l&#39;elemento Subject su [https://saml.marketo.com/sp](https://saml.marketo.com/sp)
* Se state federando più iscrizioni Marketo allo stesso provider SSO, potete utilizzare URL SP univoci per ogni sottomodulo Marketo con il formato `https://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo supporta solo i provider di identità (denominati anche IdP) avviati, in cui l&#39;utente avvia per la prima volta la pagina di accesso Idp, si autentica e quindi passa a My Marketo.

## Note aggiuntive {#additional-notes}

* **Tempo**  di sincronizzazione: per un nuovo utente, si verifica circa 10 minuti di ritardo prima dell&#39;elaborazione di una richiesta SSO iniziale.
* **Provisioning**  utente: il provisioning degli utenti viene eseguito manualmente da Marketo.
* **Autorizzazione**  - Le autorizzazioni utente vengono mantenute in Marketing Cloud.
* **Supporto**  OAuth: Marketo non supporta attualmente OAuth.

>[!NOTE]
>
>Prima di iniziare, chiedete al vostro certificato del provider di identità il formato X.509 e l&#39;estensione .crt, .der o .cer.

## Aggiorna impostazioni SAML {#update-saml-settings}

SSO è disattivato per impostazione predefinita. Segui i passaggi per abilitare SAML e configurarlo.

1. Accedere a **Admin** e fare clic su **Single Sign-On**.

   ![](assets/image2014-9-24-14-3a36-3a50.png)

   >[!NOTE]
   >
   >Se non trovi **Single Sign-On** in **Admin**, contatta [[Supporto marketing]](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Nella sezione **Impostazioni SAML** fare clic su **Modifica**.

   ![](assets/image2014-9-24-14-3a37-3a3.png)

1. Cambia **Single Sign-On** SAML in **Abilitato**.

   ![](assets/image2014-9-24-14-3a37-3a17.png)

1. Immettete l&#39; **ID emittente**, **ID entità**, selezionate la **Posizione ID utente**, quindi fate clic su **Sfoglia**.

   ![](assets/image2014-9-24-14-3a37-3a32.png)

1. Selezionare il file **Certificato provider di identità**.

   ![](assets/image2014-9-24-14-3a38-3a8.png)

1. Fare clic su **Salva**.

   ![](assets/image2014-9-24-14-3a38-3a22.png)

## Aggiorna impostazioni pagina di reindirizzamento {#update-redirect-page-settings}

1. Nella sezione **Reindirizza pagine**, fare clic su **Modifica**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >I clienti che utilizzano l&#39;ID universale insieme a SSO devono immettere l&#39;URL di accesso del provider di identità nel campo **URL di accesso**.

1. Immettere un **URL di disconnessione**. Questo è l&#39;URL a cui si desidera indirizzare l&#39;utente quando esce da Marketo.

   ![](assets/eight.png)

1. Immettere un **URL errore**. Questo è l&#39;URL a cui si desidera indirizzare l&#39;utente nel caso in cui l&#39;accesso a Marketo non riesca. Fare clic su **Salva**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Entrambe le pagine devono essere accessibili al pubblico.
