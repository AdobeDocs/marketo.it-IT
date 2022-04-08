---
description: Accesso a informazioni sulle vendite - Documenti Marketo - Documentazione del prodotto
title: Rimuovi accesso a informazioni sulle vendite
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Rimuovi accesso a informazioni sulle vendite {#remove-sales-insight-access}

Utilizza i seguenti passaggi per rimuovere l’accesso alle funzioni Approfondimenti vendite di Salesforce. Applicabile a Salesforce Classic e Lightning.

## Panoramica {#overview}

Per accedere a tutte le funzioni di Sales Insight è necessaria l’autorizzazione per gli oggetti indicati di seguito, le classi apex e le pagine di visualizzazione. La rimozione di questi elementi rimuoverà l&#39;accesso a Sales Insight.

**Impostazioni oggetto**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza Tutto, Modifica Tutto</td> 
  </tr> 
  <tr> 
   <td>Dettagli della visualizzazione delle migliori scommesse</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza Tutto, Modifica Tutto</td> 
  </tr> 
  <tr> 
   <td>Visualizzazioni migliori</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza Tutto, Modifica Tutto</td> 
  </tr> 
  <tr> 
   <td>EmailActivityCache</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza Tutto, Modifica Tutto</td> 
  </tr> 
  <tr> 
   <td>GetMethodArgus</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza Tutto, Modifica Tutto</td> 
  </tr> 
  <tr> 
   <td>GroupedWebActivityCache</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza Tutto, Modifica Tutto</td> 
  </tr> 
  <tr> 
   <td>InteressanteMomentsCache</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza Tutto, Modifica Tutto</td> 
  </tr> 
  <tr> 
   <td>Configurazione di Marketo Sales Insight</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza Tutto, Modifica Tutto</td> 
  </tr> 
  <tr> 
   <td>ScoringCache</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza Tutto, Modifica Tutto</td> 
  </tr> 
  <tr> 
   <td>Valori</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza Tutto, Modifica Tutto</td> 
  </tr> 
  <tr> 
   <td>WebActivityCache</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza Tutto, Modifica Tutto</td> 
  </tr> 
 </tbody> 
</table>

* Accesso classe Apex: 159 Classi Apex che essendo con &quot;mkto_si&quot;
* Accesso a una pagina di visualizzazione: 64 Pagine di visualizzazione con &quot;mkto_si&quot;
* Definizioni di impostazione personalizzate: Impostazioni mkto_si.Marketo e preferenze utente mkto_si.User

## Rimozione dell&#39;accesso a Sales Insight {#removing-access-to-sales-insight}

1. Accedi al tuo account Salesforce.

1. Fai clic su **Configurazione**.

   ![](assets/remove-sales-insight-access-1.png)

1. In Amministratore, fai clic su **Gestione utenti**, quindi **Profili**.

1. Fai clic sul profilo da aggiornare, quindi **Modifica**.

1. Scorri verso il basso fino a &quot;Impostazioni tabulazione personalizzate&quot; in Impostazioni scheda.

1. Selezionare l&#39;opzione &quot;Tab Hidden&quot; dal menu a discesa per Marketo Sales Insight Config e MSI Marketo Sales Outbox.

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. Scorri verso il basso fino a &quot;Autorizzazioni oggetto personalizzate&quot;.

1. Rimuovere l&#39;accesso &quot;Read, Create, Edit, Delete&quot; dai seguenti oggetti:

   * BestBetsCache
   * Dettagli della visualizzazione delle migliori scommesse
   * Visualizzazioni migliori
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InteressanteMomentsCache
   * Configurazione di Marketo Sales Insight
   * ScoringCache
   * Valori
   * WebActivityCache

1. Scorri verso il basso fino alla sezione &quot;Accesso alla classe Apex abilitato&quot;. Fai clic su **Modifica**.

1. Dalla sezione &quot;Classi apex abilitate&quot;, seleziona tutte le classi che iniziano con &quot;mkto_si&quot;. Questo dovrebbe aggiungere fino a 159 classi.

1. Fai clic su **Rimuovi**, quindi **Salva**.

   ![](assets/remove-sales-insight-access-4.png)

1. Scorri verso il basso fino alla sezione &quot;Abilitazione dell’accesso a una pagina di visualizzazione&quot;. Fai clic su **Modifica**.

1. Nella sezione &quot;Pagine di visualizzazione abilitate&quot;, seleziona tutte le pagine che iniziano con &quot;mkto_si&quot;. Questo dovrebbe aggiungere fino a 64 pagine.

1. Fai clic su **Rimuovi**, quindi **Salva**.

   ![](assets/remove-sales-insight-access-5.png)

1. Scorri verso il basso fino alla sezione &quot;Accesso alle definizioni di impostazione personalizzata abilitata&quot;. Fai clic su **Modifica**.

1. Selezionare &quot;Impostazioni Marketo Sales Insight.mkto_si.Marketo&quot; e &quot;Preferenze Marketo Sales Insight.mkto_si.User&quot;.

1. Fai clic su **Rimuovi**, quindi **Salva**.

   ![](assets/remove-sales-insight-access-6.png)

Tutto qui! L&#39;accesso a Sales Insight è stato rimosso correttamente. Ripeti gli stessi passaggi per qualsiasi altro profilo per cui desideri rimuovere l’accesso.
