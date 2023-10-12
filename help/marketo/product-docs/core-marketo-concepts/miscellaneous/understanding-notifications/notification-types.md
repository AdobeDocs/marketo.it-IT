---
unique-page-id: 2953243
description: Tipi di notifica - Documentazione di Marketo - Documentazione del prodotto
title: Tipi di notifica
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
source-git-commit: 0abb315be0f9cb5f42fa41d72b446de8c2f62c1e
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 1%

---

# Tipi di notifica {#notification-types}

Esistono diversi tipi di notifica.

## Campagna non riuscita  {#campaign-failure}

Gli errori delle campagne ti avvisano se si verificano errori nelle campagne intelligenti.

## Sincronizzazione CRM {#crm-sync}

Le notifiche di sincronizzazione CRM segnalano problemi critici rilevati durante la sincronizzazione CRM, ad esempio autorizzazioni non corrette o sincronizzazione inattiva.

**[!DNL Microsoft Dynamics]**

Le notifiche Dynamics vengono inviate una volta ogni 24 ore e contengono lead che non sono stati sincronizzati in tale periodo di tempo. I motivi tipici dell’errore sono lead duplicati (come sopra) o errori di mancata corrispondenza della lunghezza del campo.

![](assets/image2016-1-20-11-3a19-3a58.png)

**[!DNL Salesforce]**

Se utilizzi Salesforce, le notifiche di errore di sincronizzazione avranno un aspetto simile a quello riportato di seguito. Gli errori tipici includono credenziali scadute e il superamento dei limiti API.

![](assets/salesforcesyncerror.png)

## Coinvolgimento {#engagement}

Quando le persone si esauriscono in un flusso, inviamo una notifica. La notifica include il numero di persone che si sono esaurite e altre informazioni.

![](assets/image2014-10-14-10-3a57-3a9.png)

## Facebook {#facebook}

Se tenti di inviare persone a Facebook senza accettare i termini di servizio o se tenti di inviare persone a Facebook dopo aver rimosso l’app Marketo.

## Pulizia campagna attivazione inattività {#idle-trigger-campaign-cleanup}

Disattiva le campagne intelligenti attivate che non ricevono più alcuna attività. Ulteriori informazioni su  [pulizia automatica delle campagne trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

## LinkedIn {#linkedin}

Quando Marketo non è in grado di creare un nuovo pubblico, accedi o invia e-mail a LinkedIn dopo tre tentativi.

![](assets/linkedin.png)

## Servizi Web {#web-services}

Riceverai una notifica quando raggiungerai la tua quota giornaliera. La quota viene ripristinata ogni notte a mezzanotte, ora centrale.

>[!NOTE]
>
>Alcuni dei codici di errore che potresti ricevere sono descritti nel nostro [Documentazione per gli sviluppatori](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes).
