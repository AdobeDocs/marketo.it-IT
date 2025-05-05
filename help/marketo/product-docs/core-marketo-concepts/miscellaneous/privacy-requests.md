---
description: Richieste di accesso a dati personali - Documentazione di Marketo - Documentazione del prodotto
title: Richieste di accesso a dati personali
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: 0abb315be0f9cb5f42fa41d72b446de8c2f62c1e
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# Richieste di accesso a dati personali {#privacy-requests}

Questo documento fornisce una panoramica sulla gestione delle singole richieste di privacy dei dati che puoi inviare al Marketo Engage tramite l’interfaccia utente di Privacy Service e l’API di Privacy Service.

>[!NOTE]
>
>Le richieste di accesso a dati personali inviate tramite l’interfaccia utente o l’API di Privacy Service per il Marketo Engage si applicano solo ai seguenti elementi:
>
>* Utenti del Marketo Engage che hanno effettuato l’onboarding in Adobe Identity Management System
>
>**o-**
>
>* Utenti del Marketo Engage che utilizzano un altro prodotto di Experience Cloud Adobe già presente in Identity Management System (ad esempio, edizioni RT-CDP, B2B e B2P, Audience Manager).

Puoi inviare singole richieste di accesso ed eliminazione dei dati dei consumatori dal Marketo Engage in due modi:

* Tramite l&#39;[interfaccia utente Privacy Service](https://privacyui.cloud.adobe.io/). Consulta la documentazione [qui](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html?lang=it){target="_blank"}.
* Tramite l’API Privacy Service. Consulta la documentazione [qui](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target="_blank"} e le informazioni API [qui](https://developer.adobe.com/experience-platform-apis/){target="_blank"}.

[Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html?lang=it){target="_blank"} supporta due tipi di richieste: accesso ai dati ed eliminazione dei dati.

Vediamo come creare richieste di accesso ed eliminazione.

## Configurazione necessaria per inviare richieste per il Marketo Engage {#required-setup-to-send-requests-for-marketo-engage}

Per richiedere l&#39;accesso e l&#39;eliminazione dei dati per il Marketo Engage, è necessario:

1. Identificare quanto segue:

   a. ID organizzazione IMS<br/>
b. Indirizzo e-mail della persona su cui desideri agire

   Un ID organizzazione IMS è una stringa alfanumerica composta da 24 caratteri a cui segue @AdobeOrg. Se il team marketing o l&#39;amministratore di Adobe interno non conosce l&#39;ID organizzazione IMS dell&#39;organizzazione, contatta l&#39;Assistenza clienti Adobe all&#39;indirizzo `gdprsupport@adobe.com`. Per inviare richieste all’API per la privacy è necessario l’ID organizzazione IMS.

1. In Privacy Service, puoi inviare le richieste di accesso ed eliminazione al Marketo Engage e controllare lo stato delle richieste esistenti.

## Valori campo obbligatori nelle richieste JSON di Marketo Engage {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContexts&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: `<Your IMS Org ID Value>`

&quot;users&quot; (utenti):

* &quot;action&quot;: **access** o **delete**
* &quot;userIDs&quot;:
   * &quot;namespace&quot;: **email**
   * &quot;type&quot;: **standard**
   * &quot;value&quot;: `<Data Subject's Email Address>`

&quot;include&quot;:

* **marketo** (prodotto di Adobe applicabile alla richiesta)

&quot;regolamento&quot;:

* **gdpr**, **ccpa**, **pdpa**, **lgpd_bra** o **nzpa_nzl** (normativa sulla privacy applicabile alla richiesta)

## Esempio 1: richiesta di eliminazione RGPD {#gdpr-delete-request}

Richiesta JSON

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "delete"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "gdpr",
}
```

Risposta JSON

```text
{
  "requestId": "16331241037112570RX-245",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "997b01e3-9568-402c-904b-b4e60a437875",
      "customer": {
        "user": {
          "action": [
            "delete"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

## Esempio 2: richiesta di accesso CCPA {#ccpa-access-request}

Richiesta JSON

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "access"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "ccpa",
}
```

Risposta JSON

```text
{
  "requestId": "16329573462631890RX-207",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "3115e42d-011b-47ab-a2b0-ed4356af4d3e",
      "customer": {
        "user": {
          "action": [
            "access"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

>[!MORELIKETHIS]
>
>[Gestione della privacy](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md)
