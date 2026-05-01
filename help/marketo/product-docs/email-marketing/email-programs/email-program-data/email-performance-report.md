---
unique-page-id: 2359467
description: Scopri come creare e utilizzare il rapporto Prestazioni e-mail. Tieni traccia di aperture, clic, mancati recapiti e altre metriche e-mail.
title: Rapporto sulle prestazioni e-mail
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 95%

---

# Rapporto sulle prestazioni e-mail {#email-performance-report}

Per scoprire quanto sono efficaci le tue e-mail tramite statistiche quali consegnate, aperte, cliccate, ecc., crea un Rapporto sulle prestazioni e-mail.

1. [Crea un rapporto in un programma](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) e seleziona il **[!UICONTROL Email Performance]** [Tipo di rapporto](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Modifica l’intervallo di tempo del rapporto](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) e fai clic sulla scheda **[!UICONTROL Report]**.
1. Tu ci sei! Ora puoi esplora il rapporto per vedere le prestazioni delle tue e-mail.

   >[!NOTE]
   >
   >Il filtro Data di invio si basa sulla prima data in cui l’e-mail è stata inviata.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Fai clic sul nome di un’e-mail per aprirla in Anteprima e-mail.

   >[!NOTE]
   >
   >Un rapporto sulle prestazioni e-mail include le attività di tutte le persone, incluse quelle che sono state eliminate dopo l’invio dell’e-mail. A volte, potresti voler visualizzare le attività solo per le persone attive. In tal caso, è necessario escludere le persone eliminate dal rapporto tramite un filtro. Utilizza la scheda **[!UICONTROL Smart List]** per [creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) per il rapporto. Se non stai filtrando in base a nessun campo specifico, imposta il filtro Indirizzo e-mail su: **[!UICONTROL is not empty]**.

   Le [colonne del rapporto selezionate](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) per un rapporto sulle prestazioni e-mail includono:

   <table><thead>

<tr>
    <th>Colonna</th>
    <th>Descrizione</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Non recapitata in modo permanente</td>
    <td>L’e-mail è stata rifiutata a causa di una condizione permanente, ad esempio un indirizzo e-mail inesistente.</td>
  </tr>
  <tr>
    <td>Non recapitata in modo non permanente</td>
    <td>L’e-mail è stata rifiutata a causa di una condizione temporanea, ad esempio un server fuori servizio o una casella in entrata piena.</td>
  </tr>
  <tr>
    <td>In sospeso</td>
    <td>Questo numero viene calcolato sottraendo il numero di e-mail Consegnate, Non recapitate e Non recapitate in modo non permanente dal numero totale inviato.</td>
  </tr>
  <tr>
    <td>Collegamento cliccato</td>
    <td>Numero di destinatari e-mail che hanno fatto clic su un collegamento nell’e-mail.</td>
  </tr>
  <tr>
    <td>Iscrizioni annullate</td>
    <td>Numero di destinatari e-mail che hanno fatto clic sul collegamento Annulla iscrizione nell’e-mail e compilato il modulo.</td>
  </tr>
  <tr>
    <td>Interrotte</td>
    <td>Numero di e-mail che non è stato possibile recapitare e per le quali non è stato ricevuto alcun evento di mancato recapito. Un’e-mail viene automaticamente definita Interrotta se non viene ricevuta una risposta entro tre giorni dall’invio.</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>I clic sui collegamenti e sugli indirizzi e-mail per l’annullamento dell’iscrizione in un’e-mail non verranno registrati in Collegamenti cliccati nel rapporto.

In linea generale, queste statistiche vengono registrate seguendo criteri di buon senso. Ad esempio, se qualcuno ha fatto clic su un collegamento in un’e-mail, è ovvio che l’abbia prima aperta. Per il rapporto sulle prestazioni e-mail, vengono seguite le regole specifiche:

* **Regola 1**: ciascun record di attività e-mail è impostato esclusivamente su uno dei seguenti stati: _Consegnato_, _Non recapitato in modo permanente_, _Non recapitato in modo non permanente_ o _In sospeso_.

* **Regola 2**: se il record e-mail mostra _[!UICONTROL Opened]_, viene conteggiato come_ Consegnato _.

* **Regola 3**: se il record e-mail mostra _[!UICONTROL Clicked Email]_&#x200B;o_[!UICONTROL Unsubscribed]_, viene conteggiato come _Consegnato_ e _Aperto_.

* **Regola 4**: se l’e-mail è _[!UICONTROL Opened]_, i mancati recapiti vengono ignorati. Se l’e-mail non è stata aperta,_ Non recapitata in modo permanente _ha la precedenza su_ Non recapitata in modo non permanente _e_ Consegnata _.

* **Regola 5**: se non viene ricevuta alcuna attività e-mail tre giorni dopo l’invio, verrà considerata _Interrotta_.

>[!NOTE]
>
>* Più invii dalla stessa campagna alla stessa persona vengono conteggiati una sola volta.
>
>* Più invii da campagne diverse alla stessa persona vengono conteggiati separatamente.

>[!MORELIKETHIS]
>
>* [Filtrare le risorse nei rapporti e-mail di una campagna](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md){target="_blank"}
>* [Filtrare i record eliminati/uniti in un rapporto prestazioni e-mail](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-deleted-merged-records-email-performance-report.md){target="_blank"}
>* [Rapporto sulle prestazioni del collegamento e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md){target="_blank"}
