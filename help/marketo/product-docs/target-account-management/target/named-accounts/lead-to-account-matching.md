---
unique-page-id: 11381156
description: Corrispondenza lead a account - Documenti Marketo - Documentazione del prodotto
title: Corrispondenza lead a conto
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Lead per corrispondenza account {#lead-to-account-matching}

La corrispondenza a destra conduce a account con nome destro utilizzando la corrispondenza lead-to-account Marketo.

>[!NOTE]
>
>**La funzione di** corrispondenza lead-to-account è incorporata nella gestione degli account di Marketo Target. Utilizza una logica confusa per far corrispondere automaticamente i lead ai giusti account denominati in tempo quasi reale. Questi account denominati potrebbero essere account CRM o società Marketo.

La corrispondenza lead-to-conto di Marketo segue un processo in 4 fasi:

**Passaggio 1:** il processo di corrispondenza inizia utilizzando le informazioni chiave sui record lead, ad esempio:

* Dominio e-mail (ad esempio, acme.com)
* Nome della società oggetto dell’offerta dall’indirizzo IP
* Nome società: potrebbe essere il nome dell’account CRM o l’attributo del nome della società principale (ad esempio, proveniente dalla compilazione del modulo)

**Passaggio 2:** normalizziamo i nomi aziendali che troviamo in base a vari attributi di lead (ad esempio, Acme Inc. e Acme Corp vengono normalizzati automaticamente in Acme). Questo passaggio ci assicura una singola rappresentazione dell’account denominato in Marketo e può visualizzare tutti i lead all’interno di un singolo account denominato.

**Passaggio 3 -** Suddividiamo i lead abbinati in 2 blocchi: Corrispondenza forte e Corrispondenza debole.

* I lead con corrispondenza debole vengono visualizzati sugli account denominati e possono quindi essere risolti manualmente.

**Passo 4 -** Presentiamo una lista di aziende proposte con forti e deboli corrispondenze. Quando un account denominato viene creato in base a una delle società proposte, creiamo regole di corrispondenza per associare automaticamente nuovi lead (ad esempio, lead ha compilato un modulo) andando avanti verso i giusti account denominati. In questo modo puoi preoccuparti meno della corrispondenza dei lead e più di ottenere ricavi!

Poiché la corrispondenza lead-to-account Marketo è una funzione integrata di Gestione account di Target Marketo, la corrispondenza dei lead ai conti avviene in tempo quasi reale (ad esempio, nel momento in cui un lead compila un modulo Marketo, associamo il lead con il nome giusto). Questo evento può essere utilizzato per attivare gli avvisi e avvisare i proprietari dell&#39;account dei nuovi lead che arrivano dai loro account denominati.

>[!NOTE]
>
>Se utilizzi LeanData in Salesforce per eseguire la corrispondenza lead-to-account, Marketo dispone di un’integrazione che sincronizza queste corrispondenze con la tua istanza Marketo. Per abilitare questa funzione, contatta il [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Scopri account](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
