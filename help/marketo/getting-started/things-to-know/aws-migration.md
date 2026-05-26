---
description: Migrazione AWS - Documentazione Marketo Engage - Documentazione del prodotto
title: Migrazione AWS
feature: Getting Started
hide: true
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 5a260c00311588c3a55f176e7a7977f422bcc8a4
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 1%

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

* **Rivedi e aggiorna i inserisce nell&#39;elenco Consentiti di accesso, accesso API, invio di e-mail, tracciamento web e integrazioni di IP**.

* **Aggiungi i seguenti indirizzi IP** e mantieni gli IP correnti così come sono:

   * 54.160.246.246
   * 54.237.141.197
   * 52.20.211.99

## Impatto previsto sui servizi

Gli impatti riportati di seguito non richiedono alcuna azione da parte tua.

* **Le integrazioni CRM e i servizi LaunchPoint** verranno disabilitati, ma dovrebbero riprendere automaticamente in seguito.
* **Le pagine di destinazione, i moduli e la raccolta dati** non saranno disponibili e verrà visualizzato un messaggio di manutenzione.

## Pianificazione {#schedule}

Vengono aggiunte periodicamente nuove date e informazioni sui data center/pod, quindi controlla qui per ulteriori dettagli.

Prima di esaminare la tabella seguente, [scopri come identificare](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify) il centro dati e il pod/server in cui si trova la sottoscrizione.

<table>
 <tbody>
  <tr>
   <th style="width:75%">Data</th>
   <th style="width:25%">Pod</th>
  </tr>
  <tr>
   <td>5 giugno 2026</td>
   <td>AB46</td>
  </tr>
  <tr>
   <td>8 luglio 2026</td>
   <td>AB69<br>
   AB64</td>
  </tr>
  <tr>
   <td>9 luglio 2026</td>
   <td>AB70<br>
   AB43</td>
  </tr>
  &lt;/body>
  </table>

## Aggiornamenti e supporto

Per gli ultimi aggiornamenti, aggiungi un segnalibro a questa pagina. In caso di domande, contatta il supporto Adobe tramite il portale di supporto in Admin Console o [Experience League](https://experienceleague.adobe.com/it/support).
