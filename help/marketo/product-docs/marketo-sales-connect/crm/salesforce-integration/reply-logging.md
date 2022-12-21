---
unique-page-id: 14352480
description: Registrazione delle risposte (SFDC) - Documenti Marketo - Documentazione del prodotto
title: Registrazione delle risposte (SFDC)
exl-id: 11f84157-55b7-42a7-81d0-f5848adbb9f4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Registrazione delle risposte (SFDC) {#reply-logging-sfdc}

Sales Connect vi offre la possibilità di registrare automaticamente le risposte dei vostri potenziali clienti a Salesforce. La struttura che ti consente di eseguire questa operazione si basa sul nostro tracciamento delle risposte via e-mail. Se possiamo tenere traccia della risposta di un potenziale cliente, possiamo registrare tale risposta a Salesforce.

## Requisiti {#requirements}

* È necessario registrare le e-mail tramite la registrazione API
* Deve essere in grado di [tenere traccia della risposta](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
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
   >Non sarà necessario selezionare un valore predefinito nell’elenco di selezione Tipo. Sales Connect noterà che questo tipo di attività è disponibile nella tua istanza Salesforce e compila di conseguenza il campo attività sulle attività in arrivo.
