---
description: Richieste sulla privacy - Documenti Marketo - Documentazione del prodotto
title: Richieste sulla privacy
source-git-commit: 9285b1545c1cf27fb1c8579981bdf93d0cc4ff09
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Richieste sulla privacy {#privacy-requests}

Questo documento fornisce una panoramica sulla gestione delle singole richieste di privacy dei dati che è possibile inviare a Marketi Engage tramite l’interfaccia utente di Privacy Service e **API Privacy Service**.

Puoi inviare singole richieste di accesso e cancellazione dei dati dei consumatori dal Marketo Engage in due modi:

* Attraverso il [Interfaccia utente di Privacy Service](https://privacyui.cloud.adobe.io/). Consulta la documentazione [qui](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html#!api-specification/markdown/narrative/tutorials/privacy_service_tutorial/privacy_service_ui_tutorial.md).
* Attraverso il **API Privacy Service**. Consulta la documentazione [qui](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html#!api-specification/markdown/narrative/tutorials/privacy_service_tutorial/privacy_service_api_tutorial.md) e il riferimento API [qui](https://www.adobe.io/apis/experiencecloud/gdpr/api-reference.html#!acpdr/swagger-specs/privacy-service.yaml).

La [Privacy Service](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html) supporta due tipi di richieste: accesso ai dati ed eliminazione dei dati.

Nota: Le richieste di privacy inviate tramite l’interfaccia utente o l’API di Privacy Service per Marketo Engage si applicano solo ai clienti con Marketo Engage + RT-CDP, B2B e le edizioni B2P.

Vediamo come creare le richieste di accesso ed eliminazione.

## Configurazione necessaria per inviare richieste di Marketo Engage {#required-setup-to-send-requests-for-marketo-engage}

Per richiedere ad Marketo Engage l&#39;accesso e l&#39;eliminazione dei dati, devi:

1. Identifica quanto segue:

   a) ID organizzazione IMS<br/>
b) Indirizzo e-mail della persona su cui desideri agire

   Un ID organizzazione IMS è una stringa alfanumerica composta da 24 caratteri, con l&#39;aggiunta di @AdobeOrg. Se il team marketing o l’amministratore di sistema di Adobe interno non conosce l’ID organizzazione IMS della tua organizzazione, contatta l’Assistenza clienti Adobe all’indirizzo gdprsupport@adobe.com. Per inviare richieste all’API Privacy è necessario l’ID organizzazione IMS.

1. In Privacy Service è possibile inviare le richieste di accesso ed eliminazione al Marketo Engage e controllare lo stato delle richieste esistenti.

## Valori campo obbligatori nelle richieste JSON di Marketo Engage {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContexts&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: `<Your IMS Org ID Value>`

&quot;utenti&quot;:

* &quot;key&quot;: `<Your Request Tracking Key>`   (facoltativo)
* &quot;action&quot;: o **accesso** o **delete**
* &quot;userIDs&quot;:
   * &quot;namespace&quot;: **email**
   * &quot;type&quot;: **standard**
   * &quot;value&quot;: `<Data Subject’s Email Address>`

&quot;include&quot;:

* **marketo** (che è il prodotto Adobe che si applica alla richiesta)

&quot;regolamento&quot;:

* **rgpd**, **ccpa**, **pdpa**, **lgpd** oppure **nzpa**  (regolamento sulla privacy applicabile alla richiesta)

## Esempio 1: Richiesta di cancellazione RGPD {#gdpr-delete-request}

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
      "key": "AAGDPRO1", 
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
          "key": "AAGDPRO1",
          "action": [
            "delete"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": " john.doe@adobe.com",
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

## Esempio 2: Richiesta di accesso CCPA {#ccpa-access-request}

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
      "key": "AAGDPRO1",
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
      "jobId": " 3115e42d-011b-47ab-a2b0-ed4356af4d3e",
      "customer": {
        "user": {
          "key": "AAGDPRO1",
          "action": [
            "access"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": " john.doe@adobe.com",
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
