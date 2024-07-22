---
unique-page-id: 10099102
description: Rilasci di plug-in per Microsoft Dynamics MSI - Documentazione di Marketo - Documentazione del prodotto
title: Versioni dei plug-in per Microsoft Dynamics MSI
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
feature: Microsoft Dynamics
source-git-commit: 6dcda9b86555c17b3492a02f3985db7d2acd8a32
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Versioni dei plug-in per Microsoft Dynamics MSI {#plug-in-releases-for-microsoft-dynamics-msi}

La prima volta che esegui la sincronizzazione con Microsoft Dynamics, scarichi e installi la versione più recente dei plug-in per Marketo Sales Insight (MSI). Periodicamente, il Marketo Engage aggiorna questi plug-in, in modo da poter tornare nella stessa posizione per scaricare la nuova versione.

Se utilizzi la soluzione di sincronizzazione CRM nativa di Marketo per Dynamics, [scarica l&#39;ultimo plug-in](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target="_blank"} corrispondente alla versione di Dynamics. Per coloro che hanno una sincronizzazione personalizzata e hanno acquistato Marketo Sales Insight, il pacchetto [è qui](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.

>[!NOTE]
>
>Queste versioni funzionano sia per le versioni on-premise che per quelle online di Dynamics.

## Aggiornamento della soluzione MSI {#upgrading-your-msi-solution}

1. Importa la versione più recente della soluzione _sulla versione esistente_ di Dynamics CRM premendo il pulsante **[!UICONTROL Importa]** in Dynamics.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Esempio: se la versione di Dynamics CRM è 2.0.0.20 e la versione più recente è 2.0.0.21, puoi importare _over_ versione 2.0.0.20.

1. Fai clic su **[!UICONTROL Avanti]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Seleziona **[!UICONTROL Fase per l&#39;aggiornamento]** e **[!UICONTROL Gestisci personalizzazioni]**, quindi fai clic su **[!UICONTROL Importa]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Fai clic su **[!UICONTROL Avanti]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. Dopo un’importazione corretta, vedrai due soluzioni MSI: MarketoSalesInsight e MarketoSalesInsight_Upgrade. Seleziona la soluzione precedente e fai clic su Applica aggiornamento soluzione.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

Ed è tutto! Dopo l’aggiornamento verrà visualizzata una sola soluzione MSI.

## Aggiornamenti delle versioni {#version-updates}

<table> 
 <tbody> 
  <tr> 
   <th>Data di rilascio</th> 
   <th>Versione</th> 
   <th>Note</th> 
  </tr>
  <tr> 
   <td>02/14/24</td> 
   <td>2.00.31</td> 
   <td>Modifiche all’impaginazione nell’attività web anonima.
   <p>
   Crittografa le informazioni della chiave segreta dalla vista utente. Per poter eseguire la crittografia, è necessario modificare la password dopo l’importazione del nuovo pacchetto.</td> 
  </tr>
  <tr> 
   <td>10/18/23</td> 
   <td>2.00.30</td> 
   <td>Consolidamento del registro errori MSI e rimozione delle notifiche di informazioni dalla visualizzazione nell'entità errore Marketo.</td> 
  </tr>
  <tr> 
   <td>05/19/23</td> 
   <td>2.00.29</td> 
   <td>Sono stati risolti i problemi di paginazione di Attività web e Momenti di interesse nella dashboard globale.</td> 
  </tr>
  <tr> 
   <td>03/23/23</td> 
   <td>2.00.28</td> 
   <td>È stato creato un <a href="https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip">nuovo pacchetto</a> per MSI per le connessioni non native al CRM.</td> 
  </tr>
  <tr> 
   <td>02/03/22</td> 
   <td>2.0.0.27</td> 
   <td>Layout account per approfondimenti: momenti di interesse, modifiche del punteggio, attività web, attività e-mail.</td> 
  </tr>
  <tr> 
   <td>01/05/22</td> 
   <td>2.0.0.26</td> 
   <td>Punteggio di adozione del programma per l’invio di e-mail.</td> 
  </tr>
  <tr> 
   <td>10/28/21</td> 
   <td>2.0.0.25</td> 
   <td>Metriche del punteggio di adozione del prodotto, nuova dashboard globale (attività web, e-mail, elementi di maggiore rilevanza).</td> 
  </tr>
  <tr> 
   <td>02/10/21</td> 
   <td>2.0.0.22</td> 
   <td>Rimuovi il controllo automatico abilitato e le modifiche alla documentazione nella soluzione MSI.</td> 
  </tr>
  <tr> 
   <td>10/01/20</td> 
   <td>2.0.0.21</td> 
   <td>Correzione bug: assegnazione dell’accesso ai campi di configurazione dell’API MSI per gli utenti con il ruolo Sales Insight.</td> 
  </tr> 
  <tr> 
   <td>07/20/20</td> 
   <td>2.0.0.20</td> 
   <td>Correzione bug: aggiungi un messaggio di convalida per i record non sincronizzati.</td> 
  </tr> 
  <tr> 
   <td>06/12/20</td> 
   <td>2.0.0.19</td> 
   <td>Correzione bug: per nascondere la password segreta MSI nella configurazione API MSD.</td> 
  </tr> 
  <tr> 
   <td>05/26/20</td> 
   <td>2.0.0.18</td> 
   <td>Correzione bug: per modificare la convalida dell'ID ruolo MSI per la visualizzazione dei pulsanti MSI.</td> 
  </tr> 
  <tr> 
   <td>05/21/20</td> 
   <td>2.0.0.17</td> 
   <td>Correzione bug: scopri il campo proprietario e i campi non sono obbligatori.</td> 
  </tr> 
  <tr> 
   <td>04/28/20</td> 
   <td>2.0.0.16</td> 
   <td>Correzione bug: rimozione della dipendenza del collegamento per l'impostazione della mappa del sito di CRM MSD.</td> 
  </tr> 
 </tbody> 
</table>
