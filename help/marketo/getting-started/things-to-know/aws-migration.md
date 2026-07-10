---
description: Migrazione AWS - Documentazione Marketo Engage - Documentazione del prodotto
title: Migrazione AWS
feature: Getting Started
hide: true
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 3073a443b5dee8033e88dc474989c44552851e52
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 2%

---

# Migrazione AWS {#aws-migration}

Nei prossimi mesi, tutti gli abbonamenti Marketo Engage verranno migrati da un data center privato al cloud pubblico AWS per migliorare l’affidabilità, la scalabilità e la velocità.

Riceverai un’e-mail e una notifica in-app circa 30 giorni prima della migrazione. Utilizza questa guida per preparare.

## Azioni consigliate {#actions}

Durante la finestra di migrazione, tutti i servizi Marketo Engage non saranno disponibili. Per mitigare l’impatto sull’azienda, consigliamo di effettuare le seguenti operazioni.

* **Evita di creare o aggiornare lead/persone** o di eseguire processi che modificano i record Persona.

* **Non attivare i processi di follow-on**, poiché le campagne pianificate verranno sospese.

* **Disattivare temporaneamente le integrazioni** che inviano o ricevono dati da o verso Marketo Engage.

* **Evita di eseguire** importazioni o esportazioni di dati o qualsiasi campagna principale di generazione di lead/persone.

* **Rivedi e aggiorna i inserisce nell&#39;elenco Consentiti di accesso, accesso API, invio di e-mail, tracciamento web e integrazioni di IP**.

* **Aggiungi nuovi indirizzi IP** e mantieni invariati gli IP correnti. Visualizza gli indirizzi IP da aggiungere tramite la [tabella seguente](#ip-addresses).

## Impatto previsto sui servizi {#impacts}

Gli impatti riportati di seguito non richiedono alcuna azione da parte tua.

* **Le integrazioni CRM e i servizi LaunchPoint** verranno disabilitati, ma dovrebbero riprendere automaticamente in seguito.
* **Le pagine di destinazione, i moduli e la raccolta dati** non saranno disponibili e verrà visualizzato un messaggio di manutenzione.

## Identificazione del centro dati/pod {#identify}

Prima di esaminare le tabelle seguenti, [scopri come identificare](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify) il centro dati e il pod/server in cui si trova la sottoscrizione.

## Pianificazione {#schedule}

Vengono aggiunte periodicamente nuove date e informazioni sul datacenter/pod, quindi controlla qui per ulteriori dettagli.

<table>
 <tbody>
  <tr>
   <th style="width:50%">Data</th>
   <th style="width:20%">Data center/pod</th>
   <th style="width:30%">Ora</th>
  </tr>
  <tr>
   <td>8 luglio 2026</td>
   <td>AB69<br>
   AB64</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
  </tr>
  <tr>
   <td>9 luglio 2026</td>
   <td>AB70</td>
   <td>17:00 PDT</td>
  </tr>
  <tr>
   <td>11 luglio 2026</td>
   <td>AB46</td>
   <td>10:00 PDT</td>
  </tr>
  <tr>
   <td>13 luglio 2026</td>
   <td>NLD101</td>
   <td>10:00 PDT</td>
  </tr>
  <tr>
   <td>15 luglio 2026</td>
   <td>NLD102<br>
   NLD104</td>
   <td>10:00 PDT<br>
   11:00 PDT</td>
  </tr>
  <tr>
   <td>17 luglio 2026</td>
   <td>NLD103<br>
   NLD105</td>
   <td>10:00 PDT<br>
   11:00 PDT</td>
  </tr>
  <tr>
   <td>21 luglio 2026</td>
   <td>AB54<br>
   AB56</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
  </tr>
  <tr>
   <td>23 luglio 2026</td>
   <td>AB48</td>
   <td>17:00 PDT</td>
  </tr>
  <tr>
   <td>31 luglio 2026</td>
   <td>AB43</td>
   <td>15:00 PDT</td>
  </tr>
  <tr>
   <td>12 agosto 2026</td>
   <td>AB61<br>
   AB17</td>
   <td>15:00 PDT<br>
   16:00 PDT</td>
  </tr>
  <td>13 agosto 2026</td>
   <td>AB62<br>
   AB68</td>
   <td>15:00 PDT<br>
   16:00 PDT</td>
  </tr>
  </body>
</table>

## Indirizzi IP da aggiungere {#ip-addresses}

In base al centro dati, collabora con il reparto IT per aggiungere i rispettivi indirizzi IP.

<table>
<tbody>
<tr>
  <th style="width:25%">Data center</th>
  <th style="width:75%">Indirizzi IP</th>
</tr>
<tr>
  <td>AB</td>
  <td>54.160.246.246<br>
  54.237.141.197<br>
  52.20.211.99</td>
</tr>
<tr>
  <td>NLD</td>
  <td>34.247.24.245<br>
18.200.201.81<br>
54.220.138.65</td>
</tr>
</body>
</table>

## Aggiornamenti e supporto {#support}

Per gli ultimi aggiornamenti, aggiungi un segnalibro a questa pagina. In caso di domande, contatta il supporto Adobe tramite il portale di supporto in Admin Console o [Experience League](https://experienceleague.adobe.com/it/support){target="_blank"}.
