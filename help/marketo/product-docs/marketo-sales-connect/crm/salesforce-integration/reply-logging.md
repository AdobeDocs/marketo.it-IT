---
unique-page-id: 14352480
description: Registrazione delle risposte (SFDC) - Documenti Marketo - Documentazione del prodotto
title: Registrazione risposte (SFDC)
translation-type: tm+mt
source-git-commit: f28ff1acb0090892bdb92b75ef90d489db7abf20
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# Registrazione risposte (SFDC) {#reply-logging-sfdc}

Il servizio di vendita Connect vi offre la possibilità di registrare automaticamente le risposte dei potenziali clienti a Salesforce. La struttura che consente di eseguire questa operazione si basa sul nostro tracciamento delle risposte via e-mail. Se riusciamo a monitorare la risposta di un potenziale, possiamo registrare tale risposta a Salesforce.

## Requisiti {#requirements}

* È necessario registrare le e-mail tramite la registrazione API
* Deve essere in grado di [monitorare una risposta](http://docs.marketo.com/x/BYPS)
* Deve essere collegato a Salesforce
* Devono essere disponibili chiamate [](http://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) API Salesforce

## Abilita registrazione risposte {#enable-reply-logging}

1. Per abilitare la registrazione delle risposte, puoi passare alla pagina delle impostazioni [di](http://docs.marketo.com/pages/assets/external-link.jspa) Salesforce. Una volta che la registrazione API è stata disattivata, si vedrà l&#39;opzione per controllare *Risposte log.\
   *

   >[!NOTE]
   >
   >La registrazione delle risposte segue le stesse regole in vigore per la registrazione delle e-mail inviate. Ciò include il modo in cui vengono registrati i messaggi e-mail; a lead e contatti; quando esiste un duplicato del record; se non vengono trovati record corrispondenti.

## Impostazione del tipo su Rispondi in Salesforce {#setting-type-to-reply-in-salesforce}

Ottenere dati significativi dai tuoi rapporti Salesforce è importante. La possibilità di compilare il campo Tipo come &#39;Rispondi&#39; consente di ottenere tali dati attraverso i rapporti. Collaborate con voi `Salesforce admin` per ottenere questa configurazione.

1. Vai a **Setup **> **Customize **> **Activities **> Campi **** attività.
1. Fate clic su **Tipo**.
1. In Valori elenco puntato Tipo attività fare clic su **Nuovo**.
1. Digitare &quot;Rispondi&quot; nella casella vuota. Accertatevi di utilizzare il carattere maiuscolo per &quot;R&quot; e fate clic su **Salva**.

   >[!NOTE]
   >
   >Non sarà necessario selezionare un valore Predefinito nell&#39;elenco di selezione Tipo. In Sales Connect questo tipo di attività è disponibile nell&#39;istanza Salesforce e il campo attività viene compilato di conseguenza sulle attività in arrivo.

