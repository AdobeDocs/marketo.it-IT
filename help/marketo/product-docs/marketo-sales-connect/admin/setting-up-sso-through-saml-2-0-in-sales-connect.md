---
unique-page-id: 14352405
description: Impostazione di SSO tramite SAML 2.0 in Sales Connect - Marketo Docs - Documentazione del prodotto
title: Impostazione di SSO tramite SAML 2.0 in Sales Connect
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Impostazione di SSO tramite SAML 2.0 in Sales Connect {#setting-up-sso-through-saml-in-sales-connect}

Supportiamo SSO tramite la specifica SAML 2.0. Tuttavia, al momento non disponiamo di integrazioni dirette con alcun provider. Per ottenere questa configurazione, dovremo raccogliere alcune informazioni dal provider SSO.

>[!NOTE]
>
>Questo è applicabile solo a **Marketo Sales Connect** utenti. Se non disponi di Sales Connect ma desideri saperne di più, contatta il team Adobe Account (il tuo Account Manager).

## Requisiti {#requirements}

* Account SSO
* abbonamento a Marketo Sales connect
* Metadata.xml dall&#39;account SSO (URL del problema, l&#39;endpoint per la convalida e una chiave pubblica)

## Configurazione {#setup}

Il file metadata.xml dell&#39;istanza SSO del team deve contenere l&#39;URL dell&#39;emittente, l&#39;endpoint per la convalida e una chiave pubblica.

Avremo anche bisogno della posizione SSO perché l&#39;account SSO della tua azienda sia un dominio unico. Ad esempio, abbiamo bisogno di un sottodominio univoco come `toutapp.pingidentity.com` o simili. Senza questo tipo di identificatore univoco, non sarà possibile impostare SAML dal dashboard.

Un accesso e Okta non sempre forniscono identificatori univoci quando si assegna un URL. Se utilizzi Okta o One Login significa che non saremo in grado di impostare un login dal pulsante del dashboard. Sarà comunque possibile configurarlo dal pulsante Single Sign On nella [applicazione web](https://toutapp.com/login).

Una volta che avremo queste informazioni, lavoreremo con il nostro team di ingegneri per impostare questo per il tuo abbonamento.
