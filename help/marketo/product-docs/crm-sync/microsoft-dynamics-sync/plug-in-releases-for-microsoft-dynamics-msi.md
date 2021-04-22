---
unique-page-id: 10099102
description: Versioni dei plug-in per Microsoft Dynamics MSI - Documenti Marketo - Documentazione del prodotto
title: Versioni dei plug-in per Microsoft Dynamics MSI
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 4%

---

# Versioni dei plug-in per Microsoft Dynamics MSI {#plug-in-releases-for-microsoft-dynamics-msi}

La prima volta che esegui la sincronizzazione con Microsoft Dynamics, scarica e installa la versione più recente dei plug-in per Marketo Sales Insight (MSI). Marketo aggiorna periodicamente questi plug-in, in modo da poter tornare alla stessa posizione in cui scaricare la nuova versione.

Scarica l’ultimo plug-in ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) corrispondente alla versione di Dynamics.[

>[!NOTE]
>
>Queste versioni funzionano sia per le versioni on-premise che online di Dynamics.

## Aggiornamento della soluzione MSI {#upgrading-your-msi-solution}

1. Importa la versione più recente della soluzione _sulla versione esistente_ di Dynamics CRM premendo il pulsante **Importa** in Dynamics.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Esempio: se Dynamics CRM dispone della versione 2.0.0.20 e la versione più recente è 2.0.0.21, importerai _oltre_ versione 2.0.0.20.

1. Fare clic su **Avanti**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Seleziona **Stage per l&#39;aggiornamento** e **Gestisci personalizzazioni**, quindi fai clic su **Importa**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Fare clic su **Avanti**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. Dopo un&#39;importazione di successo vedrete due soluzioni MSI: MarketoSalesInsight e MarketoSalesInsight_Upgrade. Selezionare la soluzione precedente e fare clic su Applica aggiornamento soluzione.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

Ed è tutto! Dopo l&#39;aggiornamento verrà visualizzata una sola soluzione MSI.

## Aggiornamenti della versione {#version-updates}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">Data di rilascio</th> 
   <th colspan="1">Versione</th> 
   <th colspan="1">Note</th> 
  </tr> 
  <tr> 
   <td colspan="1">01/10/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">Correzione bug: Assegnazione dell'accesso ai campi di configurazione dell'API MSI per gli utenti con il ruolo Insight vendite</td> 
  </tr> 
  <tr> 
   <td colspan="1">20/07/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">Correzione bug: Aggiungere un messaggio di convalida per i record non sincronizzati</td> 
  </tr> 
  <tr> 
   <td colspan="1">12/06/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">Correzione bug: Per nascondere la password segreta MSI nella configurazione API MSD</td> 
  </tr> 
  <tr> 
   <td colspan="1">26/05/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">Correzione bug: Per modificare la convalida ID ruolo MSI per la visualizzazione dei pulsanti MSI</td> 
  </tr> 
  <tr> 
   <td colspan="1">21/05/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">Correzione bug: Mostra campo proprietario e rende i campi non obbligatori</td> 
  </tr> 
  <tr> 
   <td colspan="1">28/04/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">Correzione bug: Rimozione della dipendenza dal collegamento di impostazione del sito CRM MSD in corso</td> 
  </tr> 
 </tbody> 
</table>
