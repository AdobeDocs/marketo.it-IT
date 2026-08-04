---
description: Migrazione AWS - Documentazione Marketo Engage - Documentazione del prodotto
title: Migrazione AWS
feature: Getting Started
hide: true
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 16ff6c279c222f3cd2d9b8a1a7bbba15472231cb
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 6%

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

>[!NOTE]
>
>Se utilizzi [moduli esterni](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"} e desideri conservare i dati durante la migrazione, contatta il [supporto Adobe](https://experienceleague.adobe.com/it/support){target="_blank"} e fornisci l&#39;ID modulo e l&#39;ID Munchkin della sottoscrizione.

## Identificazione del centro dati/pod {#identify}

Prima di esaminare le tabelle seguenti, [scopri come identificare](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify) il centro dati e il pod/server in cui si trova la sottoscrizione.

## Pianificazione {#schedule}

Le nuove date e le informazioni relative al centro dati/pod vengono aggiunte o modificate periodicamente, pertanto è necessario monitorare questa pianificazione per eventuali aggiornamenti.

+++Pianificazione di luglio
<table>
 <tbody>
  <tr>
   <th style="width:25%">Data</th>
   <th style="width:25%">Data center/pod</th>
   <th style="width:25%">Ora</th>
   <th style="width:25%">Stato</th>
  </tr>
  <tr>
   <td>8 luglio 2026</td>
   <td>AB69<br>
   AB64</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Completato<br>
   Completato</td>
  </tr>
  <tr>
   <td>9 luglio 2026</td>
   <td>AB70</td>
   <td>17:00 PDT</td>
   <td>Completato</td>
  </tr>
  <tr>
   <td>11 luglio 2026</td>
   <td>AB46</td>
   <td>10:00 PDT</td>
   <td>Completato</td>
  </tr>
  <tr>
   <td>13 luglio 2026</td>
   <td>NLD101</td>
   <td>10:00 PDT</td>
   <td>Completato</td>
  </tr>
  <tr>
   <td>15 luglio 2026</td>
   <td>NLD102<br>
   NLD104</td>
   <td>10:00 PDT<br>
   11:00 PDT</td>
   <td>Completato<br>
   Completato</td>
  </tr>
  <tr>
   <td>17 luglio 2026</td>
   <td>NLD103<br>
   NLD105</td>
   <td>10:00 PDT<br>
   11:00 PDT</td>
   <td>Completato<br>
   Completato</td>
  </tr>
  <tr>
   <td>21 luglio 2026</td>
   <td>AB54</td>
   <td>17:00 PDT</td>
   <td>Completato</td>
  </tr>
  <tr>
   <td>23 luglio 2026</td>
   <td>AB48</td>
   <td>17:00 PDT</td>
   <td>Completato</td>
  </tr>
  <tr>
   <td>31 luglio 2026</td>
   <td>AB43</td>
   <td>15:00 PDT</td>
   <td>Completato</td>
  </tr>
  </body>
</table>

+++

<table>
 <tbody>
  <tr>
   <th style="width:25%">Data</th>
   <th style="width:25%">Data center/pod</th>
   <th style="width:25%">Ora</th>
   <th style="width:25%">Stato</th>
  </tr>
  <tr>
   <td>12 agosto 2026</td>
   <td>AB61<br>
   AB17</td>
   <td>15:00 PDT<br>
   16:00 PDT</td>
   <td>Secondo pianificazione<br>
   Nei tempi previsti</td>
  </tr>
  <tr>
  <td>13 agosto 2026</td>
   <td>AB68</td>
   <td>16:00 PDT</td>
   <td>Secondo pianificazione</td>
  </tr>
  <tr>
  <td>18 agosto 2026</td>
   <td>AB39</td>
   <td>17:00 PDT</td>
   <td>Secondo pianificazione</td>
  </tr>
  <tr>
   <td>20 agosto 2026</td>
   <td>AB42<br>
   AB44</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Secondo pianificazione<br>
   Nei tempi previsti</td>
  </tr>
  <tr>
   <td>26 agosto 2026</td>
   <td>AB40<br>
   AB50</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Secondo pianificazione<br>
   Nei tempi previsti</td>
  </tr>
  <tr>
   <td>28 agosto 2026</td>
   <td>AB53<br>
   AB56</td>
   <td>15:00 PDT<br>
   16:00 PDT</td>
   <td>Secondo pianificazione<br>
   Nei tempi previsti</td>
  </tr>
  <tr>
   <td>8 settembre 2026</td>
   <td>AB01<br>
   AB02</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Secondo pianificazione<br>
   Nei tempi previsti</td>
  </tr>
  <tr>
   <td>10 settembre 2026</td>
   <td>AB03<br>
   AB04</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Secondo pianificazione<br>
   Nei tempi previsti</td>
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

## Domande frequenti {#faq}

**Dove sono memorizzati i dati?**
Tutti i dati utente di Marketo vengono memorizzati su Amazon Web Services (AWS). Marketo ha trasferito la propria infrastruttura dai data center fisici di proprietà alla piattaforma cloud di livello enterprise di AWS.

**Dove vengono memorizzati i dati personali in modo specifico?**
I dati personali vengono memorizzati in Amazon Aurora, il servizio di database relazionale completamente gestito di AWS. Aurora replica i dati in sei modi in tre aree di disponibilità separate all&#39;interno dell&#39;area AWS per proteggere i dati personali da guasti hardware, deterioramento dello storage ed eventi dell&#39;infrastruttura localizzata.

**A chi appartiene l&#39;ambiente di archiviazione?**
L&#39;infrastruttura di storage è di proprietà e gestita da Amazon Web Services (AWS). Adobe (Marketo) opera come cliente di AWS secondo un modello di responsabilità condivisa: AWS è responsabile della sicurezza e della disponibilità dell’infrastruttura sottostante, mentre Adobe è responsabile della sicurezza dei dati e delle applicazioni in esecuzione al suo interno.

**Quali sono i dettagli completi su produzione, percorsi di backup/ripristino di emergenza e tecnologia di storage?**
Marketo utilizza Amazon Aurora, un motore di database relazionale nativo per il cloud completamente gestito da AWS, come tecnologia di database primaria. Aurora separa il calcolo e lo storage, replicando automaticamente i dati in sei modi in tre aree di disponibilità all&#39;interno dell&#39;area di produzione e richiedendo un quorum di quattro copie per confermare qualsiasi operazione di scrittura.

Aurora esegue inoltre backup continui e automatici su Amazon S3 in tempo reale, consentendo il ripristino point-in-time (PITR) in qualsiasi secondo all&#39;interno della finestra di conservazione configurata.

Al momento, l&#39;implementazione di Marketo per Aurora opera all&#39;interno di un&#39;unica area geografica AWS, senza replica tra aree geografiche diverse. I dati di produzione rimangono all&#39;interno dell&#39;infrastruttura regionale designata e il ripristino di emergenza viene fornito tramite la ridondanza dello storage AZ multiplo di Aurora e backup continui, anziché il failover geografico su un&#39;area secondaria. Questo aspetto può essere ulteriormente valutato con la maturazione dell’infrastruttura AWS di Marketo.
