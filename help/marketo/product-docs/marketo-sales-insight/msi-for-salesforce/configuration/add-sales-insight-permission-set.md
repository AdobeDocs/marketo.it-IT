---
description: Aggiungi set di autorizzazioni Sales Insight - Documentazione Marketo - Documentazione del prodotto
title: Aggiungi set di autorizzazioni di Sales Insight
exl-id: b93ddf2e-0f7b-41e0-ba88-7363f5e34970
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---

# Aggiungi set di autorizzazioni di Sales Insight {#add-sales-insight-permission-set}

Segui questi passaggi per aggiungere l’accesso alle funzioni di approfondimento sulle vendite in Salesforce. Applicabile a Salesforce Classic e Illuminazione

>[!PREREQUISITES]
>
>[Aggiorna il pacchetto Sales Insight Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} alla versione 1.8000 o successiva per utilizzare questa funzione.

>[!IMPORTANT]
>
>Se in precedenza hai dato a Sales Insight l’accesso a tutti i profili e/o implementato Sales Insight per tutti gli utenti, devi [rimuovi accesso a livello di profilo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} per utilizzare questo set di autorizzazioni.

## Panoramica {#overview}

L’autorizzazione &quot;App Marketo&quot; fa parte del pacchetto Sales Insight Salesforce. Include l’accesso agli oggetti menzionati di seguito, alle classi apex e alle pagine visualforce. Questi sono necessari per accedere a tutte le funzioni di Sales Insight.

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

## Aggiunta del set di autorizzazioni dell’app Marketo agli utenti {#adding-marketo-app-permission-set-to-users}

1. Accedi al tuo account Salesforce.

1. Clic **Configurazione**.

   ![](assets/add-sales-insight-permission-set-1.png)

1. In Amministratore, fai clic su per annullare **Gestisci utenti**, quindi **Utenti**.

   ![](assets/add-sales-insight-permission-set-2.png)

1. In Tutti gli utenti, seleziona l’utente a cui desideri fornire l’accesso, quindi fai clic su **Assegnazioni set di autorizzazioni**.

   ![](assets/add-sales-insight-permission-set-3.png)

1. Clic **Modifica assegnazioni**.

   ![](assets/add-sales-insight-permission-set-4.png)

1. Seleziona **Accesso all&#39;app Marketo** dai set di autorizzazioni disponibili, quindi **Aggiungi**. Clic **Salva**.

   ![](assets/add-sales-insight-permission-set-5.png)

1. Ora, quando scorri verso il basso la pagina User Detail (Dettagli utente), in Permission Set Assignments (Assegnazioni set di autorizzazioni) viene visualizzato &quot;Marketo App Access&quot; (Accesso app).

   ![](assets/add-sales-insight-permission-set-6.png)

>[!NOTE]
>
>Gli utenti che non hanno accesso a Sales Insight visualizzeranno questo messaggio: &quot;Non hai privilegi sufficienti per accedere a questa scheda.&quot;

Tutto qui! Hai aggiunto correttamente l&#39;accesso a Sales Insight. Ripeti gli stessi passaggi per qualsiasi altro profilo per il quale desideri aggiungere l’accesso.
