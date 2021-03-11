---
unique-page-id: 42762409
description: Pagina Informazioni sulle vendite per gli amministratori di Marketo - Documenti Marketo - Documentazione del prodotto
title: Pagina Approfondimenti vendite per gli amministratori di Marketo
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---


# Pagina Informazioni sulle vendite per gli amministratori di Marketo {#sales-insight-page-for-marketo-admins}

Gli amministratori di Marketo dispongono di alcuni privilegi in Sales Insight. Scopri cosa sono sotto.

## Configurazione API Soap {#soap-api-configuration}

Queste credenziali vengono utilizzate per collegare il tuo account Salesforce alla tua istanza Marketo, al fine di utilizzare MSI in Salesforce.

![](assets/one-1.png)

## Configurazione API di ripristino {#rest-api-configuration}

Queste credenziali vengono utilizzate per collegare il tuo account Salesforce alla tua istanza Marketo, al fine di utilizzare il Dashboard di MSI Insights in Salesforce.

![](assets/two-1.png)

È possibile scegliere di rimuovere le credenziali API Rest in SFDC e utilizzare solo le API Soap. Questo disattiverà il dashboard Approfondimenti

![](assets/three-1.png)

## Impostazioni punteggio persona {#person-score-settings}

* **Stelle**: Le stelle rappresentano il punteggio di lead totale rispetto ad altri lead.
* **Fiamma**: Le fiamme rappresentano l&#39;urgenza - quanto è cambiato di recente il punteggio di un lead.

Per impostazione predefinita, in Marketing Sales Insight viene utilizzato il campo Lead Score per calcolare le stelle e le fiamme. Ma se vuoi scegliere un campo diverso, ecco come:

1. Nell&#39;area **Amministratore** di Marketo, fare clic su **Informazioni sulle vendite**.

   ![](assets/four.png)

1. In Impostazioni punteggio lead fai clic su **Modifica**.

   ![](assets/five.png)

1. Seleziona il campo da utilizzare per le stelle.

   ![](assets/six.png)

1. Selezionare il campo da utilizzare per le fiamme.

   ![](assets/seven.png)

1. Fare clic su **Salva**. Le informazioni sulle vendite richiederanno un po&#39; di tempo per ricalcolare. Puoi controllare il tuo CRM più tardi per vedere le stelle e le fiamme.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Se non disponi già dei campi di valutazione personalizzati, scopri come [crearli](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[Stelle e fiamme](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## Impostazioni {#settings}

![](assets/nine.png)

**Annulla sottoscrizione impostazioni:**

Puoi scegliere tra le seguenti impostazioni di annullamento dell’abbonamento per Nessun modello, E-mail standard ed e-mail operative

* Rispetta l’impostazione Annulla sottoscrizione
* Rispetta le impostazioni di annullamento sottoscrizione quando più di un destinatario
* Rispetta le impostazioni di annullamento dell’abbonamento quando più di 5 destinatari
* Ignora impostazioni di annullamento sottoscrizione

**Abilita la possibilità di bloccare i modelli:**

Quando abilitato, gli utenti MSI non saranno in grado di modificare i modelli durante l’invio di e-mail da Salesforce

**Abilita feed RSS:**

Quando abilitato, gli utenti MSI possono visualizzare il proprio feed lead in un feed RSS (oltre al feed lead in Salesforce). Il feed RSS può funzionare solo se la funzione &quot;Scadenza token&quot; è disabilitata.

**Scadenza token:**

La scadenza del token è controllata in Feature Manager. Per attivarlo/disattivarlo, contatta il supporto di [Marketo](https://nation.marketo.com/t5/Support/ct-p/Support). Quando abilitato, tutti i token Marketo scadono entro 10 minuti. Se disabilitata, i token Marketo non scadranno.

I token generati prima dell’abilitazione della scadenza del token non avranno un tempo di scadenza per la convalida, pertanto non scadranno anche se la funzione è attualmente abilitata.

I token generati dopo l’abilitazione della scadenza del token avranno un tempo di scadenza di 10 minuti, quindi scadranno comunque in 10 minuti anche dopo la disattivazione della funzione.

Il comportamento del token si baserà su quando è stato generato (quando la funzione Scadenza token è stata abilitata/disabilitata, anziché sullo stato della funzione corrente).
