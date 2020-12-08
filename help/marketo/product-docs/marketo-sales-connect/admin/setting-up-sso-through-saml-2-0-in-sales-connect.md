---
unique-page-id: 14352405
description: Impostazione di SSO tramite SAML 2.0 in Sales Connect - Marketo Docs - Documentazione del prodotto
title: Configurazione di SSO tramite SAML 2.0 in Sales Connect
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---


# Configurazione di SSO tramite SAML 2.0 in Sales Connect {#setting-up-sso-through-saml-in-sales-connect}

Supportiamo SSO tramite la specifica SAML 2.0. Al momento, tuttavia, non disponiamo di integrazioni dirette con alcun fornitore. Per ottenere questa configurazione, è necessario raccogliere informazioni dal provider SSO.

>[!NOTE]
>
>**Promemoria**
>
>Questo è applicabile solo ai clienti **di Marketing** . Se non disponete di un servizio di vendita ma desiderate ulteriori informazioni, contattate il vostro Customer Success Manager.

## Requisiti {#requirements}

* Account SSO
* Iscrizione di Marketo Sales Connect
* Metadata.xml dall’account SSO (URL edizione, endpoint per la convalida e chiave pubblica)

## Configurazione {#setup}

Il file metadata.xml dell&#39;istanza SSO del team deve contenere l&#39;URL emittente, l&#39;endpoint per la convalida e una chiave pubblica.

Inoltre, per fare in modo che l&#39;account SSO della tua azienda sia un dominio univoco, è necessario disporre della posizione SSO. Ad esempio, a noi `require a unique subdomain` piace ‘toutapp.pingidentity.com’ o simili. Senza questo tipo di identificatore univoco, non sarà possibile impostare SAML dal dashboard.

Un login e un Okta non sempre forniscono identificatori univoci quando si assegna un URL. Se utilizzi Okta o One Login, significa che non saremo in grado di impostare un login dal pulsante del dashboard. Sarà comunque possibile configurarlo dal pulsante Single Sign On nell&#39;applicazione [](http://toutapp.com/login)Web.

Una volta ottenute tali informazioni, collaboreremo con il nostro team di progettazione per configurare l&#39;iscrizione.
