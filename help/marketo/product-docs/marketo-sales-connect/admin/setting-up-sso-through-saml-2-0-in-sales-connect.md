---
unique-page-id: 14352405
description: Impostazione di SSO tramite SAML 2.0 in Sales Connect - Documentazione di Marketo - Documentazione del prodotto
title: Impostazione di SSO tramite SAML 2.0 in Sales Connect
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Impostazione di SSO tramite SAML 2.0 in Sales Connect {#setting-up-sso-through-saml-in-sales-connect}

Supportiamo l’SSO tramite la specifica SAML 2.0. Tuttavia, al momento non disponiamo di integrazioni dirette con alcun provider. Per completare la configurazione, è necessario raccogliere alcune informazioni dal provider SSO.

>[!NOTE]
>
>Applicabile solo a **Marketo Sales Connect** utenti. Se non disponi di Sales Connect ma desideri saperne di più, contatta il team dell’account Adobe (il tuo Account Manager).

## Requisiti {#requirements}

* Account SSO
* Iscrizione a Marketo Sales Connect
* Metadata.xml dall’account SSO (URL del problema, endpoint per la convalida e chiave pubblica)

## Configurazione {#setup}

Il file metadata.xml dell’istanza SSO del team deve contenere l’URL dell’autorità di certificazione, l’endpoint per la convalida e una chiave pubblica.

Sarà inoltre necessario che la posizione SSO per l&#39;account SSO della tua azienda sia un dominio univoco. Ad esempio, è necessario un sottodominio univoco come `toutapp.pingidentity.com` o simili. Senza questo tipo di identificatore univoco, non sarà possibile impostare SAML dal dashboard.

One Login e Okta non forniscono sempre identificatori univoci quando si assegna un URL. Se utilizzi Okta o One Login significa che non sarà possibile impostare un login dal pulsante della dashboard. Sarà comunque possibile configurarlo dal pulsante Single Sign-On sulla [applicazione web](https://toutapp.com/login).

Una volta ottenute tali informazioni, collaboreremo con il nostro team di progettazione per configurarle per l’abbonamento.
