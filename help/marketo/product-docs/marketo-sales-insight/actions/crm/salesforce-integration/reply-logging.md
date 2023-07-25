---
description: Registrazione delle risposte - Documentazione di Marketo - Documentazione del prodotto
title: Registrazione delle risposte
hide: true
hidefromtoc: true
exl-id: a89e8212-83cb-4987-abc9-76c5fd74c152
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Registrazione delle risposte {#reply-logging}

Sales Insight Actions ti offre la possibilità di registrare automaticamente le risposte dei tuoi potenziali clienti a Salesforce. La struttura che ti consente di farlo si basa sul tracciamento delle risposte e-mail. Se possiamo tenere traccia della risposta di un potenziale cliente, possiamo registrare tale risposta a Salesforce.

## Requisiti {#requirements}

* Deve registrare le e-mail tramite registrazione API
* Deve essere in grado di [tracciare una risposta](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
* Deve essere collegato a Salesforce
* Deve avere Salesforce [Chiamate API](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) disponibile

## Abilita registrazione risposte {#enable-reply-logging}

1. Per abilitare la registrazione delle risposte puoi passare alla pagina delle impostazioni Salesforce. Una volta deselezionata la registrazione API, viene visualizzata l’opzione per verificare _Registra risposte_.

   >[!NOTE]
   >
   >La registrazione delle risposte segue le stesse regole in vigore per le e-mail di registrazione inviate. Ciò include il modo in cui vengono registrate le e-mail; a lead e contatti; quando esiste un record duplicato; se non vengono trovati record corrispondenti.

## Impostazione del tipo di risposta in Salesforce {#setting-type-to-reply-in-salesforce}

È importante ottenere dati significativi dai rapporti Salesforce. La possibilità di compilare il campo Tipo come &quot;Risposta&quot; consente di ottenere tali dati tramite i rapporti. Collaborate con il vostro `Salesforce admin` per ottenere questa configurazione.

1. Vai a **Configurazione** > **Personalizza** > **Attività** > **Campi attività**.
1. Clic **Tipo**.
1. In Task Type Picklist Values, fai clic su **Nuovo**.
1. Digita &quot;Reply&quot; (&quot;Risposta&quot;) nella casella vuota. Assicurarsi di scrivere la lettera &quot;R&quot; maiuscola e fare clic su **Salva**.

   >[!NOTE]
   >
   >Non è necessario selezionare un valore predefinito nell&#39;elenco a discesa Tipo. Le azioni di approfondimento sulle vendite vedranno che questo tipo di attività è disponibile nell’istanza Salesforce e compileranno di conseguenza il campo delle attività sulle attività in arrivo.
