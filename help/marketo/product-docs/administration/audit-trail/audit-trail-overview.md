---
unique-page-id: 11377945
description: Audit Trail] Panoramica - Documenti Marketo - Documentazione del prodotto
title: Panoramica di Audit Trail
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
feature: Audit Trail
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Panoramica di Audit Trail {#audit-trail-overview}

Audit Trail consente di ottenere una cronologia completa (sei mesi) delle modifiche apportate all’interno dell’istanza Marketo.

>[!NOTE]
>
>La cronologia dei dati di Audit Trail è iniziata il 14 settembre 2016.

![](assets/audit-trail-overview-1.png)

## Cos’è Audit Trail {#what-is-audit-trail}

Audit Trail acquisisce in tempo reale un elenco completo delle azioni e degli eventi che si verificano all’interno di un abbonamento Marketo. Include una modalità autonoma di accedere alla cronologia dei dati di sei mesi per poter rispondere a domande quali:

Cos’è successo a questa risorsa o impostazione e chi l’ha aggiornata per ultimo?

Cosa ha fatto l&#39;utente X?

Chi accede al nostro account?

## Cosa Controlliamo {#what-we-audit}

Marketo controllerà le azioni [crea, modifica ed elimina](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) per:

* Risorse di Design Studio
* Tutti i programmi Marketo
* Campagne intelligenti
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

Scopri chi ha effettuato l’accesso al tuo abbonamento e quando. Sono inclusi anche i tentativi di accesso non riusciti.

>[!TIP]
>
>Ci sono così tante cose che puoi controllare utilizzando Audit Trail, assicurati di utilizzare [Filtro](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)!

## Esportazione dei dati {#exporting-data}

Puoi visualizzare solo dati relativi a 30 giorni nella tua istanza. Per ottenere un valore massimo di sei mesi, utilizza l’opzione di esportazione.

![](assets/two.png)

>[!NOTE]
>
>**Definizione**
>
>**Sconosciuto:** In [!DNL Webhook], il nome e l&#39;indirizzo di posta elettronica di un utente potrebbero essere elencati come &quot;Sconosciuto&quot;. Ciò si verifica quando si apporta una modifica ai valori dell’elenco di selezione nel CRM. Questi valori vengono visualizzati nei moduli e nelle pagine di destinazione di Marketo. Effettuando questo aggiornamento sul lato CRM, le pagine di destinazione che fanno riferimento al modulo verranno automaticamente redatte. In [!DNL Webhook] verrà rilevato che la pagina di destinazione è stata creata, ma il nome e l&#39;indirizzo di posta elettronica dell&#39;utente saranno &quot;Sconosciuto&quot;, in quanto non è possibile acquisire le informazioni utente dal lato CRM.

>[!MORELIKETHIS]
>
>[Abilita prova di verifica](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
