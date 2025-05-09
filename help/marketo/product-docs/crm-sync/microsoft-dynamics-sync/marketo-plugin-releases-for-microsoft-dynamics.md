---
unique-page-id: 10099389
description: Rilasci di plug-in Marketo per Microsoft Dynamics - Documentazione di Marketo - Documentazione del prodotto
title: Rilasci di plug-in Marketo per Microsoft Dynamics
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: f1fd9564abe4702c3a124442ee26027d4d22f23d
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Rilasci di plug-in Marketo per Microsoft Dynamics {#marketo-plugin-releases-for-microsoft-dynamics}

La prima volta che esegui la sincronizzazione con Microsoft Dynamics, scarichi la versione più recente dei plug-in per Marketo. Periodicamente, Marketo aggiorna questi plug-in, in modo da poter tornare nella stessa posizione per scaricare la nuova versione.

[Scarica il plug-in più recente](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} corrispondente alla versione di Dynamics.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Aggiornamento della soluzione Dynamics {#updating-your-dynamics-solution}

1. Importa la versione più recente della soluzione rispetto alla versione esistente di Dynamics CRM (ad esempio, se la versione di Dynamics CRM è 1.4 e quella più recente è 1.5, è necessario importare _over_ versione 1.4).

1. Viene visualizzata la seguente finestra a comparsa. Seleziona **Aggiorna** e **Gestisci personalizzazioni**, quindi fai clic su **Importa**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Versioni più recenti {#latest-versions}

>[!NOTE]
>
>Queste versioni funzionano sia per le versioni on-premise che per quelle online di Dynamics.

<table> 
 <tbody> 
  <tr> 
   <th style="width:15%">Versione</th> 
   <th style="width:20%">Data di rilascio</th> 
   <th style="width:65%">Note</th> 
  </tr>
  <tr> 
   <td>5.0.2.1.</td> 
   <td>1/19/24</td> 
   <td>Correzione bug: sono stati corretti alcuni bug relativi alla sincronizzazione di entità personalizzate.</td> 
  </tr> 
  <tr> 
   <td>5.0.2.0</td> 
   <td>03/24/23</td> 
   <td>Correzione bug: sono stati corretti alcuni bug che impedivano l’unione dei contatti in MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td>5.0.1.8.</td> 
   <td>03/27/23</td> 
   <td>Correzione bug: impedisce al plug-in di sovrascrivere altre personalizzazioni sugli elementi dell’interfaccia utente in MS Dynamics.
   <p>
   Correzione bug: sono state ripristinate le sezioni di navigazione che risultavano mancanti in 5.0.1.1.</td> 
  </tr> 
  <tr> 
   <td>5.0.1.1.</td> 
   <td>02/04/21</td> 
   <td>Supporto per la sincronizzazione di campi Set di opzioni a selezione multipla (questa funzione è disponibile solo per versione 9.X e successive).</td> 
  </tr> 
  <tr> 
   <td>4.2.0.0</td> 
   <td>10/16/20</td> 
   <td>È stato aggiunto il supporto per la sincronizzazione di Campaign con MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.24</td> 
   <td>8/22/18</td> 
   <td>È stato aggiunto il supporto per il lead idoneo predefinito per il processo di contatto per Microsoft Dynamics versione 9.x.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.23</td> 
   <td>6/27/18</td> 
   <td>Correzione bug: errore del processo aziendale durante il tentativo di installare le soluzioni Marketo per Dynamics 2013.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.22</td> 
   <td>9/29/17</td> 
   <td>Correzione bug: revisione interna.</td> 
  </tr> 
  <tr> 
   <td><p>4.0.0.21</p></td> 
   <td>11/9/16</td> 
   <td>Correzione bug: il plug-in non ha sottoscritto eventi che acquisiscono la modifica dello stato dell’oggetto personalizzato. Questa correzione è specifica per Dynamics CRM On Premise 2011.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.20</td> 
   <td>7/22/16</td> 
   <td>Correzione bug: gli aggiornamenti del ruolo di contatto dell’opportunità non venivano acquisiti completamente.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.19</td> 
   <td>6/28/16</td> 
   <td>Correzione bug: al momento della creazione dell’opportunità è stata notata una transazione di aggiornamento non necessaria sul ruolo customeropportunityrole nel registro marketo.<p>Correzione bug: è stata registrata una transazione di eliminazione aggiuntiva durante l’eliminazione dell’entità customeropportunityrole.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.18</td> 
   <td>5/31/16</td> 
   <td>Correzione bug: l’aggiornamento e l’eliminazione degli oggetti personalizzati sono stati resi asincroni.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.17</td> 
   <td>4/8/16</td> 
   <td>Correzione bug: quando il lead aveva un filtro di sincronizzazione impostato su NO e l’opportunità e il contatto non avevano un filtro di sincronizzazione, il registro di creazione non veniva generato per il contatto e l’opportunità quando il lead era qualificato.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.16</td> 
   <td>3/29/16</td> 
   <td>Correzione bug: è stato registrato un evento Assign quando il filtro di sincronizzazione è stato disattivato.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.15</td> 
   <td>3/3/16</td> 
   <td>Correzione bug: il cliente non ha potuto creare un lead in CRM perché l'utente di accesso non disponeva dell'autorizzazione Configurazione Marketo.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.14</td> 
   <td>1/18/16</td> 
   <td>Correzione bug: sono stati creati limiti di accesso per gli utenti normali di Dynamics per risolvere i problemi di sicurezza.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.13</td> 
   <td>12/30/15</td> 
   <td>Correzione bug: gli aggiornamenti in Dynamics non venivano sincronizzati con Marketo per passaggi e immagini.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.12</td> 
   <td>11/12/15</td> 
   <td>Correzione bug: i record lead venivano sincronizzati in Marketo quando il filtro di sincronizzazione era impostato su false.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Scarica la soluzione Marketo per la gestione dei lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}
