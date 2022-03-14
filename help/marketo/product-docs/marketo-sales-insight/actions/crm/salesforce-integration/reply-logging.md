---
description: Registrazione delle risposte - Documenti Marketo - Documentazione del prodotto
title: Registrazione delle risposte
hide: true
hidefromtoc: true
source-git-commit: c398aff77e09f4a63db5d51af55178aa663ec98e
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Registrazione delle risposte {#reply-logging}

Azioni di Insight sulle vendite ti offre la possibilità di registrare automaticamente le risposte dei tuoi potenziali clienti a Salesforce. La struttura che ti consente di eseguire questa operazione si basa sul nostro tracciamento delle risposte via e-mail. Se possiamo tenere traccia della risposta di un potenziale cliente, possiamo registrare tale risposta a Salesforce.

## Requisiti {#requirements}

* È necessario registrare le e-mail tramite la registrazione API
* Deve essere in grado di [tenere traccia della risposta](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
* Deve essere collegato a Salesforce
* Deve avere Salesforce [Chiamate API](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) disponibile

## Abilita registrazione risposte {#enable-reply-logging}

1. Per abilitare la registrazione delle risposte, puoi passare alla pagina delle impostazioni Salesforce. Una volta che la registrazione API è stata disattivata, visualizzerai l’opzione per controllare _Risposte al registro_.

   >[!NOTE]
   >
   >La registrazione delle risposte segue le stesse regole che hai impostato per la registrazione delle e-mail inviate. Ciò include il modo in cui le e-mail vengono registrate; a Lead e contatti; quando esiste un record duplicato; se non vengono trovati record corrispondenti.

## Impostazione del tipo per la risposta in Salesforce {#setting-type-to-reply-in-salesforce}

Ottenere dati significativi dai rapporti Salesforce è importante. La possibilità di compilare il campo Tipo come &quot;Risposta&quot; consente di ottenere tali dati attraverso i rapporti. Collaborare con `Salesforce admin` per ottenere questa configurazione.

1. Vai a **Configurazione** > **Personalizza** > **Attività** > **Campi attività**.
1. Fai clic su **Tipo**.
1. In Valori elenco puntato tipo attività fare clic su **Nuovo**.
1. Digita &quot;Reply&quot; (Risposta) nella casella vuota. Assicurati di utilizzare il carattere maiuscolo per la R e fai clic su **Salva**.

   >[!NOTE]
   >
   >Non sarà necessario selezionare un valore predefinito nell’elenco di selezione Tipo. In Azioni Approfondimenti vendite questo tipo di attività è disponibile nell’istanza Salesforce e compila di conseguenza il campo attività per le attività in arrivo.
