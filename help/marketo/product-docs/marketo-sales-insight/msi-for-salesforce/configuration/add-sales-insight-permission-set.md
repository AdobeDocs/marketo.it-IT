---
description: Aggiungi set di autorizzazioni Insight per le vendite - Documentazione Marketo - Documentazione del prodotto
title: Aggiungi set di autorizzazioni Insight vendite
exl-id: b93ddf2e-0f7b-41e0-ba88-7363f5e34970
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 1%

---

# Aggiungi set di autorizzazioni [!DNL Sales Insight] {#add-sales-insight-permission-set}

Utilizzare la procedura seguente per aggiungere l&#39;accesso alle funzionalità di [!DNL Sales Insight] in [!DNL Salesforce]. Applicabile a [!DNL Salesforce] Classic e Lightening

>[!PREREQUISITES]
>
>[Aggiorna il pacchetto [!DNL Sales Insight] [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} alla versione 1.8000 o successiva per utilizzare questa funzionalità.

>[!IMPORTANT]
>
>Se in precedenza hai concesso a [!DNL Sales Insight] l&#39;accesso a tutti i profili e/o implementato [!DNL Sales Insight] per tutti gli utenti, devi [rimuovere l&#39;accesso a livello di profilo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} per utilizzare questo set di autorizzazioni.

## Panoramica {#overview}

L&#39;autorizzazione &quot;App Marketo&quot; fa parte del pacchetto [!DNL Sales Insight] [!DNL Salesforce]. Include l’accesso agli oggetti menzionati di seguito, alle classi apex e alle pagine visualforce. Questi sono necessari per accedere a tutte le funzionalità di [!DNL Sales Insight].

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
   <td>Configurazione Marketo [!DNL Sales Insight]</td>
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

## Aggiunta del set di autorizzazioni dell’app Marketo agli utenti {#adding-marketo-app-permission-set-to-users}

1. Accedi al tuo account [!DNL Salesforce].

1. Fai clic su **[!UICONTROL Setup]**.

   ![](assets/add-sales-insight-permission-set-1.png)

1. In Amministratore, fare clic per eseguire l&#39;unfurl di **[!UICONTROL Manage Users]**, quindi di **[!UICONTROL Users]**.

   ![](assets/add-sales-insight-permission-set-2.png)

1. In Tutti gli utenti selezionare l&#39;utente a cui si desidera fornire l&#39;accesso, quindi fare clic su **[!UICONTROL Permission Set Assignments]**.

   ![](assets/add-sales-insight-permission-set-3.png)

1. Fai clic su **[!UICONTROL Edit Assignments]**.

   ![](assets/add-sales-insight-permission-set-4.png)

1. Selezionare **[!UICONTROL Marketo App Access]** dai set di autorizzazioni disponibili, quindi **[!UICONTROL Add]**. Fai clic su **[!UICONTROL Save]**.

   ![](assets/add-sales-insight-permission-set-5.png)

1. Ora, quando scorri verso il basso la pagina User Detail (Dettagli utente), in Permission Set Assignments (Assegnazioni set di autorizzazioni) viene visualizzato &quot;Marketo App Access&quot; (Accesso app).

   ![](assets/add-sales-insight-permission-set-6.png)

>[!NOTE]
>
>Gli utenti che non hanno accesso a [!DNL Sales Insight] visualizzeranno questo messaggio: &quot;Non hai privilegi sufficienti per accedere a questa scheda.&quot;

Tutto qui. Hai aggiunto l&#39;accesso [!DNL Sales Insight]. Ripeti gli stessi passaggi per qualsiasi altro profilo per il quale desideri aggiungere l’accesso.
