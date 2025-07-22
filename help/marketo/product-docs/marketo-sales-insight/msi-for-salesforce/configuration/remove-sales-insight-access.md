---
description: Rimuovi l'accesso a Sales Insight - Documentazione Marketo - Documentazione del prodotto
title: Rimuovi l'accesso a Sales Insight
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 3%

---

# Rimuovi l&#39;accesso a [!DNL Sales Insight] {#remove-sales-insight-access}

Utilizzare la procedura seguente per rimuovere l&#39;accesso alle funzionalità di [!DNL Sales Insight] in [!DNL Salesforce]. Applicabile a [!DNL Salesforce] Classic e Lightning.

## Panoramica {#overview}

Per accedere a tutte le funzionalità di [!DNL Sales Insight] è necessaria l&#39;autorizzazione per gli oggetti indicati di seguito, le classi apex e le pagine visualforce. Se rimuovi questi elementi, verrà rimosso l&#39;accesso a [!DNL Sales Insight].

**Impostazioni oggetto**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza tutto, Modifica tutto</td> 
  </tr> 
  <tr> 
   <td>[!DNL Best Bets] Visualizza i dettagli</td> 
   <td>Leggi, Crea, Modifica, Elimina, Visualizza tutto, Modifica tutto</td> 
  </tr> 
  <tr> 
   <td>[!DNL Best Bets] Viste</td> 
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
   <td>[!DNL Marketo Sales Insight] Config</td> 
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

## Rimozione dell&#39;accesso a [!DNL Sales Insight] {#removing-access-to-sales-insight}

1. Accedi al tuo account [!DNL Salesforce].

1. Fai clic su **[!UICONTROL Setup]**.

   ![](assets/remove-sales-insight-access-1.png)

1. In [!UICONTROL Administrator], fare clic su **[!UICONTROL Manage Users]**, quindi su **[!UICONTROL Profiles]**.

1. Fai clic sul profilo che desideri aggiornare, quindi **[!UICONTROL Edit]**.

1. Scorri verso il basso fino a &quot;[!UICONTROL Custom Tab Settings]&quot; in [!UICONTROL Tab Settings].

1. Selezionare l&#39;opzione &quot;[!UICONTROL Tab Hidden]&quot; dal menu a discesa per la cartella di configurazione [!DNL Marketo Sales Insight] e la cartella di posta in uscita [!DNL Marketo Sales] MSI.

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. Scorri verso il basso fino a &quot;[!UICONTROL Custom Object Permissions]&quot;.

1. Rimuovi l’accesso &quot;Read, Create, Edit, Delete&quot; (Lettura, creazione, modifica, eliminazione) dai seguenti oggetti:

   * BestBetsCache
   * [!DNL Best Bets] Visualizza dettagli
   * [!DNL Best Bets] visualizzazioni
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InterestingMomentsCache
   * Configurazione [!DNL Marketo Sales Insight]
   * ScoringCache
   * Valori
   * WebActivityCache

1. Scorri verso il basso fino alla sezione &quot;[!UICONTROL Enabled Apex Class Access]&quot;. Fai clic su **[!UICONTROL Edit]**.

1. Dalla sezione &quot;[!UICONTROL Enabled Apex Classes]&quot; selezionare tutte le classi che iniziano con &quot;mkto_si&quot;. Questo dovrebbe aggiungere fino a 159 classi.

1. Fare clic su **[!UICONTROL Remove]**, quindi su **[!UICONTROL Save]**.

   ![](assets/remove-sales-insight-access-4.png)

1. Scorri verso il basso fino alla sezione &quot;[!UICONTROL Enabled Visualforce Page Access]&quot;. Fai clic su **[!UICONTROL Edit]**.

1. Dalla sezione &quot;[!UICONTROL Enabled Visualforce Pages]&quot; selezionare tutte le pagine che iniziano con &quot;mkto_si&quot;. Il totale ammonta a 64 pagine.

1. Fare clic su **[!UICONTROL Remove]**, quindi su **[!UICONTROL Save]**.

   ![](assets/remove-sales-insight-access-5.png)

1. Scorri verso il basso fino alla sezione &quot;[!UICONTROL Enabled Custom Setting Definitions Access]&quot;. Fai clic su **[!UICONTROL Edit]**.

1. Selezionare &quot;Marketo Sales Insight.mkto_si.Marketo Settings&quot; e &quot;Marketo Sales Insight.mkto_si.User Preferences&quot;.

1. Fare clic su **[!UICONTROL Remove]**, quindi su **[!UICONTROL Save]**.

   ![](assets/remove-sales-insight-access-6.png)

Tutto qui. Hai rimosso correttamente l&#39;accesso a [!DNL Sales Insight]. Ripeti gli stessi passaggi per qualsiasi altro profilo per il quale desideri rimuovere l’accesso.
