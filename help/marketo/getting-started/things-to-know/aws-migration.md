---
description: Migrazione AWS - Documentazione Marketo Engage - Documentazione del prodotto
title: Migrazione AWS
feature: Getting Started
hide: true
hidefromtoc: true
source-git-commit: 88155ad99ba2899c3db3c1f7ae92a69f348dc020
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Migrazione AWS {#aws-migration}

Nei prossimi mesi, tutti gli abbonamenti Marketo Engage verranno migrati da un data center privato al cloud pubblico AWS per migliorare l’affidabilità, la scalabilità e la velocità.

Riceverai un’e-mail e una notifica in-app circa 30 giorni prima della migrazione. Utilizza questa guida per preparare.

## Azioni consigliate

Durante la finestra di migrazione, tutti i servizi Marketo Engage non saranno disponibili. Per mitigare l’impatto sull’azienda, consigliamo di effettuare le seguenti operazioni.

* **Evita di creare o aggiornare lead/persone** o di eseguire processi che modificano i record Persona.

* **Non attivare i processi di follow-on**, poiché le campagne pianificate verranno sospese.

* **Disattivare temporaneamente le integrazioni** che inviano o ricevono dati da o verso Marketo Engage.

* **Evita di eseguire** importazioni o esportazioni di dati o qualsiasi campagna principale di generazione di lead/persone.

* **Rivedi e aggiorna i inserisce nell&#39;elenco Consentiti di IP** per l&#39;accesso, l&#39;accesso API, l&#39;invio di e-mail, il tracciamento web e le integrazioni.

* Aggiungi i seguenti indirizzi IP e mantieni gli IP correnti così come sono:

   * 54.160.246.246
   * 54.237.141.197
   * 52.20.211.99

## Impatto previsto sui servizi

Gli impatti riportati di seguito non richiedono alcuna azione da parte tua.

* **Le integrazioni CRM e i servizi LaunchPoint** verranno disabilitati, ma dovrebbero riprendere automaticamente in seguito.
* **Le pagine di destinazione, i moduli e la raccolta dati** non saranno disponibili e verrà visualizzato un messaggio di manutenzione.

## Aggiornamenti e supporto

Per gli ultimi aggiornamenti, aggiungi un segnalibro a questa pagina. In caso di domande, contatta il supporto Adobe tramite il portale di supporto in Admin Console o [Experience League](https://experienceleague.adobe.com/it/support).

DA AGGIUNGERE: DETTAGLI POD/DATA CENTER
