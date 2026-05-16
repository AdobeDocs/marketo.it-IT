---
unique-page-id: 14352405
description: Scopri come impostare l’SSO tramite SAML 2.0 in Sales Connect. Ottieni i requisiti e i passaggi di configurazione per il provider SSO e il dominio univoco.
title: Impostazione di SSO tramite SAML 2.0 in [!DNL Sales Connect]
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/FLGacQUvOJFtKJ5O1PzWRmpk3Zm1KH1D-W3ATHSVRSA
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 270
ht-degree: 0%

---

# Impostazione di SSO tramite SAML 2.0 in [!DNL Sales Connect] {#setting-up-sso-through-saml-in-sales-connect}

Supportiamo l’SSO tramite la specifica SAML 2.0. Tuttavia, al momento non disponiamo di integrazioni dirette con alcun provider. Per completare la configurazione, è necessario raccogliere alcune informazioni dal provider SSO.

>[!NOTE]
>
>Applicabile solo a **utenti Marketo Sales Connect**. Se non disponi di Sales Connect ma desideri saperne di più, contatta il team dell’account Adobe (il tuo Account Manager).

## Requisiti {#requirements}

* Account SSO
* Iscrizione a Marketo Sales Connect
* Metadata.xml dall’account SSO (URL del problema, endpoint per la convalida e chiave pubblica)

## Configurazione {#setup}

Il file metadata.xml dell’istanza SSO del team deve contenere l’URL dell’autorità di certificazione, l’endpoint per la convalida e una chiave pubblica.

Sarà inoltre necessario che la posizione SSO per l&#39;account SSO della tua azienda sia un dominio univoco. Ad esempio, è necessario un sottodominio univoco come `toutapp.pingidentity.com` o simile. Senza questo tipo di identificatore univoco, non sarà possibile impostare SAML dal dashboard.

One Login e Okta non forniscono sempre identificatori univoci quando si assegna un URL. Se utilizzi Okta o One Login significa che non sarà possibile impostare un login dal pulsante della dashboard. Sarà comunque possibile configurarlo dal pulsante Single Sign-On nell&#39;[applicazione Web](https://toutapp.com/login).

Una volta ottenute tali informazioni, collaboreremo con il nostro team di progettazione per configurarle per l’abbonamento.
