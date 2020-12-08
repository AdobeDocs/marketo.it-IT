---
unique-page-id: 11381156
description: Lead to Account Matching - Marketo Docs - Documentazione prodotto
title: Lead per corrispondenza account
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Lead per corrispondenza account {#lead-to-account-matching}

La corrispondenza a destra conduce agli account denominati a destra utilizzando la corrispondenza lead-to-account Marketo.

>[!NOTE]
>
>**La corrispondenza** lead-to-account è una funzione integrata del marketing basato su account di Marketo. Utilizza una logica sfocata per far corrispondere automaticamente i lead ai giusti account denominati in tempo quasi reale. Questi account denominati potrebbero essere account CRM o società Marketo.

L&#39;associazione tra lead e account di marketing segue un processo in 4 fasi:

**Passaggio 1 -** Il nostro processo di corrispondenza inizia utilizzando le informazioni chiave sui record principali, come:

* Dominio e-mail (ad esempio, acme.com)
* Nome società indicato dall&#39;indirizzo IP
* Nome società: può essere il nome account CRM o l&#39;attributo del nome della società lead, ad esempio proviene dalla compilazione del modulo

**Passo 2 -** Normalizziamo i nomi aziendali che troviamo in base a vari attributi principali (ad esempio Acme Inc. e Acme Corp vengono normalizzati automaticamente in Acme). Questo passaggio ci consente di avere una singola rappresentazione dell&#39;account denominato in Marketo e di visualizzare tutti i lead all&#39;interno di un singolo account denominato.

**Passaggio 3 -** Divisioni abbinate i lead in 2 bucket: Corrispondenza forte e Corrispondenza debole.

* I lead con corrispondenza debole vengono visualizzati sugli account denominati e possono quindi essere risolti manualmente.

**Passo 4 -** Presentiamo una lista di aziende proposte con forti e deboli corrispondenze. Quando un account denominato viene creato in base a una delle società proposte, vengono create regole di corrispondenza per associare automaticamente nuovi lead (ad es. lead compilato un modulo) andando avanti verso i conti denominati giusti. In questo modo puoi preoccuparti meno di trovare una corrispondenza con i lead e più di ottenere ricavi!

Poiché la corrispondenza lead-to-account di Marketo è una funzione integrata del marketing basato su account di Marketo, la corrispondenza dei lead agli account avviene quasi in tempo reale (ad esempio, nel momento in cui un lead compila un modulo di Marketo, viene associato detto lead con l’account con il nome giusto). Questo evento può essere utilizzato per attivare gli avvisi e notificare ai proprietari dell&#39;account i nuovi lead che arrivano dai loro account denominati.

>[!NOTE]
>
>Se utilizzi LeanData in Salesforce per effettuare la corrispondenza lead-to-account, Marketo dispone di un&#39;integrazione che consente di sincronizzare tali corrispondenze all&#39;istanza di Marketo. Per abilitare questa funzione, contatta il [supporto](https://nation.marketo.com/t5/Support/ct-p/Support)di Marketo.

>[!MORELIKETHIS]
>
>* [Scopri account](/help/marketo/product-docs/account-based-marketing/target/named-accounts/discover-accounts.md)

