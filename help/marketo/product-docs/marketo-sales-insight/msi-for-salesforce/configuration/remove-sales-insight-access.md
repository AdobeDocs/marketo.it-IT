---
description: Rimuovere l’accesso a Sales Insight - Documentazione di Marketo - Documentazione del prodotto
title: Rimuovi l'accesso a Sales Insight
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Rimuovi l&#39;accesso a Sales Insight {#remove-sales-insight-access}

Utilizza i seguenti passaggi per rimuovere l’accesso alle funzioni di Sales Insight in Salesforce. Applicabile a Salesforce Classic e Lightning.

## Panoramica {#overview}

Per accedere a tutte le funzioni di Sales Insight è necessaria l’autorizzazione per gli oggetti indicati di seguito, le classi apex e le pagine visualforce. Se rimuovi questi elementi, verrà rimosso l’accesso a Sales Insight.

**Impostazioni oggetto**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza tutto, Modifica tutto</td> 
  </tr> 
  <tr> 
   <td>Elementi di maggiore rilevanza Visualizza dettagli</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza tutto, Modifica tutto</td> 
  </tr> 
  <tr> 
   <td>Visualizzazioni elementi di maggiore rilevanza</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza tutto, Modifica tutto</td> 
  </tr> 
  <tr> 
   <td>EmailActivityCache</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza tutto, Modifica tutto</td> 
  </tr> 
  <tr> 
   <td>GetMethodArgus</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza tutto, Modifica tutto</td> 
  </tr> 
  <tr> 
   <td>GroupedWebActivityCache</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza tutto, Modifica tutto</td> 
  </tr> 
  <tr> 
   <td>InterestingMomentsCache</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza tutto, Modifica tutto</td> 
  </tr> 
  <tr> 
   <td>Configurazione approfondimento vendite Marketo</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza tutto, Modifica tutto</td> 
  </tr> 
  <tr> 
   <td>ScoringCache</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza tutto, Modifica tutto</td> 
  </tr> 
  <tr> 
   <td>Valori</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza tutto, Modifica tutto</td> 
  </tr> 
  <tr> 
   <td>WebActivityCache</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza tutto, Modifica tutto</td> 
  </tr> 
 </tbody> 
</table>

* Accesso alle classi Apex: 159 classi Apex che iniziano con &quot;mkto_si&quot;
* Accesso alla pagina di Visualforce: 64 pagine di Visualforce che iniziano con &quot;mkto_si&quot;
* Definizioni di impostazioni personalizzate: impostazioni mkto_si.Marketo e preferenze mkto_si.User

## Rimozione dell’accesso a Sales Insight {#removing-access-to-sales-insight}

1. Accedi al tuo account Salesforce.

1. Clic **Configurazione**.

   ![](assets/remove-sales-insight-access-1.png)

1. In Amministratore, fai clic su **Gestisci utenti**, quindi **Profili**.

1. Fai clic sul profilo da aggiornare, quindi **Modifica**.

1. Scorri verso il basso fino a &quot;Impostazioni Linguetta Customizzata&quot; in Impostazioni Linguetta.

1. Selezionare l&#39;opzione &quot;Scheda nascosta&quot; dal menu a discesa per Marketo Sales Insight Config e MSI Marketo Sales Outbox.

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. Scorri verso il basso fino a &quot;Autorizzazioni oggetto personalizzato&quot;.

1. Rimuovi l’accesso &quot;Read, Create, Edit, Delete&quot; (Lettura, creazione, modifica, eliminazione) dai seguenti oggetti:

   * BestBetsCache
   * Elementi di maggiore rilevanza Visualizza dettagli
   * Visualizzazioni elementi di maggiore rilevanza
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InterestingMomentsCache
   * Configurazione approfondimento vendite Marketo
   * ScoringCache
   * Valori
   * WebActivityCache

1. Scorri verso il basso fino alla sezione &quot;Accesso classe di apice abilitato&quot;. Clic **Modifica**.

1. Dalla sezione &quot;Classi Apex abilitate&quot;, selezionare tutte le classi che iniziano con &quot;mkto_si&quot;. Questo dovrebbe aggiungere fino a 159 classi.

1. Clic **Rimuovi**, quindi **Salva**.

   ![](assets/remove-sales-insight-access-4.png)

1. Scorri verso il basso fino alla sezione &quot;Abilitato Visualforce Page Access&quot; (Accesso pagina Visualforce abilitato). Clic **Modifica**.

1. Dalla sezione &quot;Pagine Visualforce abilitate&quot;, seleziona tutte le pagine che iniziano con &quot;mkto_si&quot;. Il totale ammonta a 64 pagine.

1. Clic **Rimuovi**, quindi **Salva**.

   ![](assets/remove-sales-insight-access-5.png)

1. Scorri verso il basso fino alla sezione &quot;Accesso alle definizioni delle impostazioni personalizzate abilitate&quot;. Clic **Modifica**.

1. Selezionare &quot;Marketo Sales Insight.mkto_si.Marketo Settings&quot; e &quot;Marketo Sales Insight.mkto_si.User Preferences&quot;.

1. Clic **Rimuovi**, quindi **Salva**.

   ![](assets/remove-sales-insight-access-6.png)

Tutto qui! Hai rimosso correttamente l&#39;accesso a Sales Insight. Ripeti gli stessi passaggi per qualsiasi altro profilo per il quale desideri rimuovere l’accesso.
