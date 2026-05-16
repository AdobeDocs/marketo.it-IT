---
unique-page-id: 42762409
description: Scopri la pagina Sales Insight per gli amministratori di Marketo. Accedi alle impostazioni di configurazione delle azioni e MSI.
title: Pagina Sales Insight per gli amministratori di Marketo
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/FTOgWRDvY14tovIUclyWrED5DBXcHXH8APcprG-DlK4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 376
ht-degree: 3%

---

# [!DNL Sales Insight] pagina per amministratori di Marketo {#sales-insight-page-for-marketo-admins}

Gli amministratori di Marketo dispongono di alcuni privilegi in [!DNL Sales Insight]. Scopri di più.

## Configurazione API Soap {#soap-api-configuration}

Queste credenziali vengono utilizzate per connettere l&#39;account [!DNL Salesforce] all&#39;istanza Marketo per utilizzare MSI in [!DNL Salesforce].

![](assets/one-1.png)

## Configurazione API REST {#rest-api-configuration}

Queste credenziali vengono utilizzate per connettere l&#39;account [!DNL Salesforce] all&#39;istanza di Marketo per utilizzare il dashboard di approfondimenti MSI in [!DNL Salesforce].

![](assets/two-1.png)

## Impostazioni punteggio persona {#person-score-settings}

* **[!UICONTROL Stars]**: le stelle rappresentano il punteggio totale del lead rispetto ad altri lead.
* **[!UICONTROL Flames]**: le fiamme rappresentano l&#39;urgenza - quanto il punteggio di un lead è cambiato di recente.

Per impostazione predefinita, [!DNL Marketo Sales Insight] utilizza il campo Punteggio lead per calcolare le stelle e le fiamme. Ma se vuoi scegliere un campo diverso, ecco come:

1. Nell&#39;area **[!UICONTROL Admin]** di Marketo, fare clic su **[!UICONTROL Sales Insight]**.

   ![](assets/four.png)

1. In [!UICONTROL Lead Scoring Settings], fare clic su **[!UICONTROL Edit]**.

   ![](assets/five.png)

1. Selezionare il campo da utilizzare per le stelle.

   ![](assets/six.png)

1. Selezionare il campo da utilizzare per le fiamme.

   ![](assets/seven.png)

1. Fai clic su **[!UICONTROL Save]**. Il ricalcolo di Sales insight richiederà del tempo. Puoi controllare il tuo CRM più tardi per vedere le stelle e le fiamme.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Se non disponi già dei campi di punteggio personalizzati, ecco come [crearli](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[Stelle e fiamme](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## Impostazioni {#settings}

![](assets/nine.png)

**Impostazioni annullamento sottoscrizione:**

Puoi scegliere una delle seguenti impostazioni per annullare l&#39;iscrizione a [!UICONTROL No Template], [!UICONTROL Standard Emails] e [!UICONTROL Operational emails]

* [!UICONTROL Respect Unsubscribe Setting]
* [!UICONTROL Respect Unsubscribe Settings when more than 1 recipient]
* [!UICONTROL Respect Unsubscribe Settings when more than 5 recipients]
* [!UICONTROL Ignore Unsubscribe Settings]

**Possibilità di bloccare i modelli:**

Se abilitata, gli utenti MSI non potranno modificare i modelli durante l&#39;invio di e-mail da [!DNL Salesforce]

**Abilita feed RSS:**

Se abilitata, gli utenti MSI possono visualizzare il proprio feed lead in un feed RSS (oltre al feed lead in [!DNL Salesforce]). Il feed RSS può funzionare solo se la funzionalità &quot;[!UICONTROL Token Expiration]&quot; è disabilitata.

**Scadenza token:**

La scadenza del token è controllata in Feature Manager. Per attivarlo o disattivarlo, contattare il [supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support). Se abilitati, tutti i token Marketo scadono entro 10 minuti. Se disabilitati, i token Marketo non scadranno.

I token generati prima dell’abilitazione della scadenza del token non avranno un tempo di scadenza per la convalida, pertanto non scadranno anche se la funzione è attualmente abilitata.

I token generati dopo l’abilitazione della scadenza del token avranno un tempo di scadenza di 10 minuti, quindi scadranno tra 10 minuti anche dopo la disabilitazione della funzione.

Il comportamento del token sarà basato su quando è stato generato (quando la funzione Scadenza token è stata abilitata/disabilitata, anziché sullo stato corrente della funzione).
