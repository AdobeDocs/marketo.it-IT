---
unique-page-id: 14352480
description: Registrazione delle risposte (SFDC) - Documenti Marketo - Documentazione del prodotto
title: Registrazione risposte (SFDC)
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Registrazione risposte (SFDC) {#reply-logging-sfdc}

Il servizio di vendita Connect vi offre la possibilità di registrare automaticamente le risposte dei potenziali clienti a Salesforce. La struttura che consente di eseguire questa operazione si basa sul nostro tracciamento delle risposte via e-mail. Se riusciamo a monitorare la risposta di un potenziale, possiamo registrare tale risposta a Salesforce.

## Requisiti {#requirements}

* È necessario registrare le e-mail tramite la registrazione API
* Deve essere in grado di [tenere traccia di una risposta](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* Deve essere collegato a Salesforce
* Deve essere disponibile una chiamata Salesforce [API](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm)

## Abilita registrazione risposte {#enable-reply-logging}

1. Per abilitare la registrazione delle risposte, puoi passare alla pagina delle impostazioni di Salesforce. Una volta disattivata la registrazione delle API, verrà visualizzata l&#39;opzione per selezionare _Risposte registro_.

   >[!NOTE]
   >
   >La registrazione delle risposte segue le stesse regole in vigore per la registrazione delle e-mail inviate. Ciò include il modo in cui vengono registrati i messaggi e-mail; a lead e contatti; quando esiste un duplicato del record; se non vengono trovati record corrispondenti.

## Impostazione del tipo per la risposta in Salesforce {#setting-type-to-reply-in-salesforce}

Ottenere dati significativi dai tuoi rapporti Salesforce è importante. La possibilità di compilare il campo Tipo come &#39;Rispondi&#39; consente di ottenere tali dati attraverso i rapporti. Per ottenere questa configurazione, è necessario collaborare con il `Salesforce admin`.

1. Andate a **Setup** > **Customize** > **Activities** > **Campi attività**.
1. Fare clic su **Tipo**.
1. In Valori elenco puntato tipo attività, fare clic su **Nuovo**.
1. Digitare &quot;Rispondi&quot; nella casella vuota. Assicurarsi di utilizzare il carattere maiuscolo &quot;R&quot; e fare clic su **Salva**.

   >[!NOTE]
   >
   >Non sarà necessario selezionare un valore Predefinito nell&#39;elenco di selezione Tipo. In Sales Connect questo tipo di attività è disponibile nell&#39;istanza Salesforce e il campo attività viene compilato di conseguenza sulle attività in arrivo.
