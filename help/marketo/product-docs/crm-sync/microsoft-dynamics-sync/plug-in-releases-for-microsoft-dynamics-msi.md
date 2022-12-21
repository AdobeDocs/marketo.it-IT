---
unique-page-id: 10099102
description: Versioni dei plug-in per Microsoft Dynamics MSI - Documenti Marketo - Documentazione del prodotto
title: Versioni dei plug-in per Microsoft Dynamics MSI
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
source-git-commit: ff076d66a193664aa6ec05cf940143cebdd2d942
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 6%

---

# Versioni dei plug-in per Microsoft Dynamics MSI {#plug-in-releases-for-microsoft-dynamics-msi}

La prima volta che esegui la sincronizzazione con Microsoft Dynamics, scarica e installa la versione più recente dei plug-in per Marketo Sales Insight (MSI). Marketo aggiorna periodicamente questi plug-in, in modo da poter tornare alla stessa posizione in cui scaricare la nuova versione.

Se utilizzi una soluzione di sincronizzazione CRM nativa di Marketo per Dynamics, ti preghiamo di: [scarica il plug-in più recente](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target=&quot;_blank&quot;} corrispondente alla versione di Dynamics. Per coloro che hanno una sincronizzazione personalizzata e hanno acquistato Marketo Sales Insight, la [il pacchetto è qui](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target=&quot;_blank&quot;}.

>[!NOTE]
>
>Queste versioni funzionano sia per le versioni on-premise che online di Dynamics.

## Aggiornamento della soluzione MSI {#upgrading-your-msi-solution}

1. Importare la versione più recente della soluzione _sulla versione esistente_ di Dynamics CRM premendo il pulsante **Importa** in Dynamics.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Esempio: se Dynamics CRM dispone della versione 2.0.0.20 e la versione più recente è 2.0.0.21, importeresti _over_ versione 2.0.0.20.

1. Fai clic su **Successivo**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Seleziona **Fase di aggiornamento** e **Gestisci personalizzazioni**, quindi fai clic su **Importa**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Fai clic su **Successivo**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. Dopo un&#39;importazione di successo vedrete due soluzioni MSI: MarketoSalesInsight e MarketoSalesInsight_Upgrade. Selezionare la soluzione precedente e fare clic su Applica aggiornamento soluzione.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

Ed è tutto! Dopo l&#39;aggiornamento verrà visualizzata una sola soluzione MSI.

## Aggiornamenti versione {#version-updates}

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
   <td colspan="1">02/03/22</td> 
   <td colspan="1">2.0.0.27</td> 
   <td colspan="1">Layout dell'account per informazioni approfondite: Momenti interessanti, modifiche al punteggio, attività web, attività e-mail</td> 
  </tr>
  <tr> 
   <td colspan="1">01/05/22</td> 
   <td colspan="1">2.0.0.26</td> 
   <td colspan="1">Punteggio di adozione del programma per l’invio di e-mail</td> 
  </tr>
  <tr> 
   <td colspan="1">10/28/21</td> 
   <td colspan="1">2.0.0.25</td> 
   <td colspan="1">Metriche punteggio di adozione del prodotto, nuovo dashboard globale (attività web, e-mail, elementi migliori)</td> 
  </tr>
  <tr> 
   <td colspan="1">02/10/21</td> 
   <td colspan="1">2.0.0.22</td> 
   <td colspan="1">Rimuovere il controllo automatico abilitato e le modifiche alla documentazione sulla soluzione MSI</td> 
  </tr>
  <tr> 
   <td colspan="1">10/01/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">Correzione bug: Assegnazione dell'accesso ai campi di configurazione dell'API MSI per gli utenti con il ruolo Insight vendite</td> 
  </tr> 
  <tr> 
   <td colspan="1">07/20/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">Correzione bug: Aggiungere un messaggio di convalida per i record non sincronizzati</td> 
  </tr> 
  <tr> 
   <td colspan="1">06/12/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">Correzione bug: Per nascondere la password segreta MSI nella configurazione API MSD</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/26/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">Correzione bug: Per modificare la convalida ID ruolo MSI per la visualizzazione dei pulsanti MSI</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/21/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">Correzione bug: Mostra campo proprietario e rende i campi non obbligatori</td> 
  </tr> 
  <tr> 
   <td colspan="1">04/28/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">Correzione bug: Rimozione della dipendenza dal collegamento di impostazione del sito CRM MSD in corso</td> 
  </tr> 
 </tbody> 
</table>
