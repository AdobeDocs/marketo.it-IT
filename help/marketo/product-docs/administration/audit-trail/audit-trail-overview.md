---
unique-page-id: 11377945
description: Panoramica di Audit Trail e come acquisisce una cronologia di sei mesi delle modifiche e dell’attività di accesso nell’istanza Marketo.
title: Panoramica su Audit trail
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
feature: Audit Trail
TQID: https://experienceleague.adobe.com/4MTpv09ZFWkX6tirnq7ZIABSkfoz07qljcUUORwYNn8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 2%

---

# Panoramica su Audit trail {#audit-trail-overview}

Audit Trail consente di ottenere una cronologia completa (sei mesi) delle modifiche apportate all’interno dell’istanza Marketo.

>[!NOTE]
>
>La cronologia dei dati di Audit Trail è iniziata il 14 settembre 2016.

![](assets/audit-trail-overview-1.png)

## Cos’è Audit Trail {#what-is-audit-trail}

Audit Trail acquisisce in tempo reale un elenco completo delle azioni e degli eventi che si verificano all’interno di un abbonamento Marketo. Include una modalità autonoma di accedere alla cronologia dei dati di sei mesi per poter rispondere a domande quali:

&quot;Cos’è successo a questa risorsa o impostazione e chi l’ha aggiornata per ultimo?&quot;

&quot;Che cosa ha fatto l’utente X?&quot;

&quot;Chi accede al nostro account?&quot;

## Cosa Controlliamo {#what-we-audit}

Marketo controlla le azioni [crea, modifica ed elimina](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) per:

* Risorse di Design Studio
* Tutti i programmi Marketo
* Campagne avanzate
* Elenchi (smart/static)
* Utenti (amministratore)
* Ruoli e autorizzazioni (amministratore)
* Workspace e partizioni (amministratore)
* Cronologia degli accessi utente

>[!NOTE]
>
>Marketo _non_ è in corso il controllo delle modifiche apportate in Web Personalization, Predictive Content o Sales Insight.

## Componenti Audit Trail {#audit-trail-components}

Audit Trail è costituito da tre componenti.

**1) [Asset Audit Trail](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

Consulta Attività eseguita su risorse specifiche.

**2) [Admin Audit Trail](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

Monitorare i dettagli basati sugli utenti.

**3) [Cronologia accesso utente](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

Scopri chi ha effettuato l’accesso alla sottoscrizione e quando (include anche i tentativi di accesso non riusciti).

>[!TIP]
>
>Dato che è possibile controllare molte cose con Audit Trail, [filtrare](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md) può essere un grande risparmio di tempo.

## Esportazione dei dati {#exporting-data}

Puoi visualizzare solo dati relativi a 30 giorni nella tua istanza. Per ottenere un valore massimo di sei mesi, utilizza l’opzione di esportazione.

![](assets/two.png)

>[!NOTE]
>
>**Definizione**
>
>**Sconosciuto:** In [!DNL Webhook], il nome e l&#39;indirizzo di posta elettronica di un utente potrebbero essere elencati come &quot;Sconosciuto&quot;. Ciò si verifica quando si apporta una modifica ai valori dell’elenco di selezione nel CRM. Questi valori vengono visualizzati nei moduli e nelle pagine di destinazione di Marketo. Effettuando questo aggiornamento sul lato CRM, le pagine di destinazione che fanno riferimento al modulo verranno automaticamente redatte. In [!DNL Webhook], Marketo rileva che la pagina di destinazione è stata creata, ma il nome e l&#39;indirizzo di posta elettronica dell&#39;utente saranno &quot;Sconosciuto&quot;, in quanto Marketo non è in grado di acquisire le informazioni utente dal lato CRM.

>[!MORELIKETHIS]
>
>[Abilita prova di verifica](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
