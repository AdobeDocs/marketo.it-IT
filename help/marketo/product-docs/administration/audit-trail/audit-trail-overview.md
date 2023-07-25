---
unique-page-id: 11377945
description: Panoramica di Audit Trail - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica di Audit Trail
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
feature: Audit Trail
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '328'
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

Marketo controllerà [creare, modificare ed eliminare](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) azioni per:

* Risorse di Design Studio
* Tutti i programmi Marketo
* Campagne intelligenti
* Elenchi (smart/static)
* Utenti (amministratore)
* Ruoli e autorizzazioni (amministratore)
* Area di lavoro e partizioni (amministratore)
* Cronologia degli accessi utente

>[!NOTE]
>
>Marketo è _non_ il controllo delle modifiche apportate in Personalizzazione web, Contenuto predittivo o Insight vendite in questo momento.

## Componenti Audit Trail {#audit-trail-components}

Audit Trail è costituito da tre componenti.

**1) [Asset Audit Trail](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

Consulta Attività eseguita su risorse specifiche.

**2) [Admin Audit Trail](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

Monitorare i dettagli basati sugli utenti.

**3) [Cronologia di accesso utente](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

Scopri chi ha effettuato l’accesso al tuo abbonamento e quando. Sono inclusi anche i tentativi di accesso non riusciti.

>[!TIP]
>
>Ci sono così tante cose che puoi controllare utilizzando Audit Trail, assicurati di utilizzare [Filtraggio](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)!

## Esportazione dei dati {#exporting-data}

Puoi visualizzare solo dati relativi a 30 giorni nella tua istanza. Per ottenere un valore massimo di sei mesi, utilizza l’opzione di esportazione.

![](assets/two.png)

>[!NOTE]
>
>**Definizione**
>
>**Sconosciuto:** In entrata [!DNL Webhook], è possibile che il nome e l’indirizzo e-mail di un utente siano elencati come &quot;Sconosciuto&quot;. Ciò si verifica quando si apporta una modifica ai valori dell’elenco di selezione nel CRM. Questi valori vengono visualizzati nei moduli e nelle pagine di destinazione di Marketo. Effettuando questo aggiornamento sul lato CRM, le pagine di destinazione che fanno riferimento al modulo verranno automaticamente redatte. In entrata [!DNL Webhook], acquisiremo che la pagina di destinazione è stata redatta, ma il nome e l’e-mail dell’utente saranno visualizzati come &quot;Sconosciuto&quot;, in quanto non siamo in grado di acquisire le informazioni utente dal lato CRM.

>[!MORELIKETHIS]
>
>[Abilita Audit Trail](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
