---
unique-page-id: 42762409
description: Pagina Informazioni sulle vendite per gli amministratori di Marketo - Marketo Docs - Documentazione sui prodotti
title: Pagina Informazioni sulle vendite per gli amministratori di marketing
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---


# Pagina Informazioni sulle vendite per gli amministratori di marketing {#sales-insight-page-for-marketo-admins}

Gli amministratori di marketing dispongono di alcuni privilegi in Sales Insight. Scopri di seguito.

## Configurazione API Soap {#soap-api-configuration}

Queste credenziali vengono utilizzate per collegare il tuo account Salesforce all&#39;istanza Marketo, al fine di utilizzare MSI in Salesforce.

![](assets/one-1.png)

## Configurazione API Rest {#rest-api-configuration}

Queste credenziali vengono utilizzate per collegare il tuo account Salesforce all&#39;istanza di Marketo, al fine di utilizzare il Dashboard approfondimenti MSI in Salesforce.

![](assets/two-1.png)

È possibile scegliere di rimuovere le credenziali Rest API in SFDC e utilizzare solo le API Soap. Questo disattiverà il dashboard Insights

![](assets/three-1.png)

## Impostazioni punteggio persona {#person-score-settings}

* **Stelle**: Le stelle rappresentano il punteggio totale del lead rispetto ad altri lead.
* **Fiamma**: Le fiamme rappresentano l&#39;urgenza - quanto è cambiato recentemente il punteggio di un lead.

Per impostazione predefinita, Marketing Sales Insight utilizza il campo Lead Score per calcolare stelle e fiamme. Ma se vuoi scegliere un campo diverso, ecco come:

1. Nell&#39;area **Admin** di Marketo, fare clic su **Sales Insight**.

   ![](assets/four.png)

1. In Impostazioni punteggio lead fare clic su **Modifica**.

   ![](assets/five.png)

1. Selezionate il campo da utilizzare per le stelle.

   ![](assets/six.png)

1. Selezionare il campo da utilizzare per le fiamme.

   ![](assets/seven.png)

1. Fare clic su **Salva**. Le informazioni sulle vendite richiederanno un po&#39; di tempo per eseguire nuovamente il calcolo. Puoi controllare il CRM in un secondo momento per vedere le stelle e le fiamme.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Se non hai già i tuoi campi di valutazione personalizzati, ecco come [crearli](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[Stelle e fiamme](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## Impostazioni {#settings}

![](assets/nine.png)

**Impostazioni di annullamento sottoscrizione:**

Potete scegliere tra le seguenti impostazioni di annullamento della sottoscrizione per Nessun modello, E-mail standard e E-mail operative

* Rispetta impostazione di annullamento sottoscrizione
* Rispetta le impostazioni di annullamento della sottoscrizione quando più di un destinatario
* Rispetta le impostazioni di annullamento della sottoscrizione quando più di 5 destinatari
* Ignora impostazioni annullamento sottoscrizione

**Abilitare il blocco dei modelli:**

Quando attivato, gli utenti MSI non saranno in grado di modificare i modelli durante l&#39;invio di e-mail da Salesforce

**Abilita feed RSS:**

Quando è attivata, gli utenti MSI possono visualizzare il proprio Feed lead in un feed RSS (oltre al Feed lead in Salesforce).
