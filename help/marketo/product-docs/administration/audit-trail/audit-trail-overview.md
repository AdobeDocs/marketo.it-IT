---
unique-page-id: 11377945
description: Panoramica della traccia di controllo - Documenti Marketo - Documentazione del prodotto
title: Panoramica della traccia di controllo
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---


# Panoramica della traccia di controllo {#audit-trail-overview}

Audit Trail consente di ottenere una cronologia completa (per sei mesi) delle modifiche apportate all’interno dell’istanza di Marketo.

>[!NOTE]
>
>La cronologia dei dati delle tracce di controllo è iniziata il 14 settembre 2016.

![](assets/one.png)

## Che cos&#39;è la traccia di controllo {#what-is-audit-trail}

La traccia di audit acquisisce, in tempo reale, un elenco completo delle azioni e degli eventi che si verificano all’interno di un’iscrizione a Marketo. Include un modo self-service per accedere a una cronologia di dati di sei mesi per rispondere a domande come:

Cos&#39;è successo a questa risorsa o impostazione e chi l&#39;ha aggiornata per ultima?

Fino a che punto è arrivato l&#39;utente X?

Chi accede al nostro account?

## Elementi di controllo {#what-we-audit}

Marketo controllerà le azioni [create, modificate ed eliminate](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail) per:

* Progettare le risorse di studio
* Tutti i programmi Marketo
* Campagne intelligenti
* Elenchi (smart/statici)
* Utenti (amministratore)
* Ruoli e autorizzazioni (amministratore)
* Area di lavoro e partizioni (amministratore)
* Cronologia login utente

>[!NOTE]
>
>Al momento, Marketo è **non** il controllo delle modifiche effettuate in Web Personalization (Personalizzazione Web), Predictive Content (Contenuto predittivo) o Sales Insight (Informazioni sulle vendite).

## Componenti della traccia di controllo {#audit-trail-components}

Audit Trail è costituito da tre componenti.

**1)  [Descrizione attività](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail#ChangeDetailsinAuditTrail-AssetAuditTrail)**

Consultate attività eseguite su risorse specifiche.

**2) Audit Trail  [Amministratore](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail#ChangeDetailsinAuditTrail-AdminAuditTrail)**

Monitorate i dettagli basati sull’utente.

**3) Cronologia login  [utente](http://docs.marketo.com/display/DOCS/User+Login+History)**

Scopri chi ha effettuato l’accesso al tuo abbonamento e quando. Sono inclusi anche i tentativi di accesso non riusciti.

>[!TIP]
>
>C&#39;è così tanto che puoi eseguire il controllo utilizzando la traccia di audit, assicurati di utilizzare [Filtering](http://docs.marketo.com/display/DOCS/Filtering+in+Audit+Trail)!

## Esportazione dati {#exporting-data}

È possibile visualizzare solo 30 giorni di dati nell&#39;istanza. Per ottenere (fino a) sei mesi, utilizzare l&#39;opzione di esportazione.

![](assets/two.png)

>[!NOTE]
>
>**Definizione**
>
>**Sconosciuto:** nella traccia di controllo, il nome e l&#39;e-mail di un utente potrebbero essere elencati come &quot;Sconosciuto&quot;. Ciò si verifica quando si apporta una modifica ai valori dell&#39;elenco di selezione in CRM. Questi valori vengono visualizzati nei moduli Marketo e nelle pagine di destinazione. Se si esegue questo aggiornamento sul lato CRM, le pagine di destinazione che fanno riferimento al modulo verranno automaticamente sbozzate. Nella traccia di audit, acquisiremo che la pagina di destinazione è stata redatta, ma il nome dell&#39;utente e l&#39;e-mail saranno visualizzati come &quot;Sconosciuto&quot;, in quanto non siamo in grado di acquisire le informazioni utente dal lato CRM.

>[!MORELIKETHIS]
>
>* [Abilita traccia di controllo](enable-audit-trail.md)

>



