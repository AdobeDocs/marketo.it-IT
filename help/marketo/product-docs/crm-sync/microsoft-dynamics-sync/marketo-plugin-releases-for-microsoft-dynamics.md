---
unique-page-id: 10099389
description: Rilasci di plug-in Marketo per Microsoft Dynamics - Documentazione di Marketo - Documentazione del prodotto
title: Rilasci di plug-in Marketo per Microsoft Dynamics
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 7%

---

# Rilasci di plug-in Marketo per Microsoft Dynamics {#marketo-plugin-releases-for-microsoft-dynamics}

La prima volta che esegui la sincronizzazione con Microsoft Dynamics, scarichi la versione più recente dei plug-in per Marketo. Periodicamente, Marketo aggiorna questi plug-in, in modo da poter tornare nella stessa posizione per scaricare la nuova versione.

[Scarica il plug-in più recente](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) corrisponde alla versione di Dynamics.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Aggiornamento della soluzione Dynamics {#updating-your-dynamics-solution}

1. Importa la versione più recente della soluzione rispetto alla versione esistente di Dynamics CRM (ad esempio, se la versione di Dynamics CRM è 1.4 e quella più recente è 1.5, puoi importare _oltre_ versione 1.4).

1. Viene visualizzata la seguente finestra a comparsa. Seleziona **Aggiorna** e **Gestisci personalizzazioni**, quindi fai clic su **Importa**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Versioni più recenti {#latest-versions}

>[!NOTE]
>
>Queste versioni funzionano sia per le versioni on-premise che per quelle online di Dynamics.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Versione</th> 
   <th colspan="1">Data di rilascio</th> 
   <th>Note</th> 
  </tr> 
  <tr> 
   <td colspan="1">5.0.1.1</td> 
   <td colspan="1">02/04/21</td> 
   <td colspan="1">Supporto per la sincronizzazione di campi Set di opzioni a selezione multipla (questa funzione è disponibile solo per versione 9.X e successive). .</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">È stato aggiunto il supporto per la sincronizzazione di Campaign con MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">È stato aggiunto il supporto per il lead idoneo predefinito per il processo di contatto per Microsoft Dynamics versione 9.x.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">6/27/18</td> 
   <td colspan="1">Correzione bug: errore del processo aziendale durante il tentativo di installare le soluzioni Marketo per Dynamics 2013.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">9/29/17</td> 
   <td colspan="1">Correzione bug: revisione interna.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">Correzione bug: il plug-in non ha sottoscritto eventi che acquisiscono la modifica dello stato dell’oggetto personalizzato. Questa correzione è specifica per Dynamics CRM On Premise 2011. </td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">7/22/16</td> 
   <td colspan="1">Correzione bug: gli aggiornamenti del ruolo di contatto dell’opportunità non venivano acquisiti completamente.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">6/28/16</td> 
   <td colspan="1"><p>Correzione bug: al momento della creazione dell’opportunità è stata notata una transazione di aggiornamento non necessaria sul ruolo customeropportunityrole nel registro marketo. </p><p>Correzione bug: è stata registrata una transazione di eliminazione aggiuntiva durante l’eliminazione dell’entità customeropportunityrole.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">5/31/16</td> 
   <td colspan="1">Correzione bug: l’aggiornamento e l’eliminazione degli oggetti personalizzati sono stati resi asincroni.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">4/8/16</td> 
   <td colspan="1">Correzione bug: quando il lead aveva un filtro di sincronizzazione impostato su NO e l’opportunità e il contatto non avevano un filtro di sincronizzazione, il registro di creazione non veniva generato per il contatto e l’opportunità quando il lead era qualificato.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">3/29/16</td> 
   <td>Correzione bug: è stato registrato un evento Assign quando il filtro di sincronizzazione è stato disattivato.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">Correzione bug: il cliente non ha potuto creare un lead in CRM perché l'utente di accesso non disponeva dell'autorizzazione Configurazione Marketo.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">1/18/16</td> 
   <td colspan="1">Correzione bug: sono stati creati limiti di accesso per gli utenti normali di Dynamics per risolvere i problemi di sicurezza.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">12/30/15</td> 
   <td>Correzione bug: gli aggiornamenti in Dynamics non venivano sincronizzati con Marketo per passaggi e immagini.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">11/12/15</td> 
   <td colspan="1">Correzione bug: i record lead venivano sincronizzati in Marketo quando il filtro di sincronizzazione era impostato su false.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Scarica la soluzione di gestione dei lead Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)
