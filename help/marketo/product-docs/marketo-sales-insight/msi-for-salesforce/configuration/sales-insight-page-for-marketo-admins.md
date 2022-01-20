---
unique-page-id: 42762409
description: Pagina Approfondimenti vendite per amministratori Marketo - Documentazione Marketo - Documentazione del prodotto
title: Pagina Approfondimenti vendite per gli amministratori Marketo
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
source-git-commit: 5812f447fbe22bee13060afae8408de7ca7384e5
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Pagina Approfondimenti vendite per gli amministratori Marketo {#sales-insight-page-for-marketo-admins}

Gli amministratori di Marketo dispongono di determinati privilegi in Sales Insight. Scopri cosa sono sotto.

## Configurazione API Soap {#soap-api-configuration}

Queste credenziali vengono utilizzate per collegare il tuo account Salesforce alla tua istanza Marketo, al fine di utilizzare MSI in Salesforce.

![](assets/one-1.png)

## Configurazione dell’API Rest {#rest-api-configuration}

Queste credenziali vengono utilizzate per collegare il tuo account Salesforce alla tua istanza Marketo, al fine di utilizzare il Dashboard di MSI Insights in Salesforce.

![](assets/two-1.png)

## Impostazioni punteggio persona {#person-score-settings}

* **Stelle**: Le stelle rappresentano il punteggio di lead totale rispetto ad altri lead.
* **Fiamma**: Le fiamme rappresentano l&#39;urgenza - quanto è cambiato di recente il punteggio di un lead.

Per impostazione predefinita, Marketo Sales Insight utilizza il campo Lead Score per calcolare le stelle e le fiamme. Ma se vuoi scegliere un campo diverso, ecco come:

1. In **Amministratore** area di Marketo, fai clic su **Approfondimenti vendite**.

   ![](assets/four.png)

1. In Impostazioni punteggio lead fai clic su **Modifica**.

   ![](assets/five.png)

1. Seleziona il campo da utilizzare per le stelle.

   ![](assets/six.png)

1. Selezionare il campo da utilizzare per le fiamme.

   ![](assets/seven.png)

1. Fai clic su **Salva**. Le informazioni sulle vendite richiederanno un po&#39; di tempo per ricalcolare. Puoi controllare il tuo CRM più tardi per vedere le stelle e le fiamme.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Se non disponi già dei campi di valutazione personalizzati, ecco come [crearle](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

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

La scadenza del token è controllata in Feature Manager. Per attivarlo/disattivarlo, contatta [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support). Quando abilitato, tutti i token Marketo scadono entro 10 minuti. Se disabilitata, i token Marketo non scadranno.

I token generati prima dell’abilitazione della scadenza del token non avranno un tempo di scadenza per la convalida, pertanto non scadranno anche se la funzione è attualmente abilitata.

I token generati dopo l’abilitazione della scadenza del token avranno un tempo di scadenza di 10 minuti, quindi scadranno comunque in 10 minuti anche dopo la disattivazione della funzione.

Il comportamento del token si baserà su quando è stato generato (quando la funzione Scadenza token è stata abilitata/disabilitata, anziché sullo stato della funzione corrente).
