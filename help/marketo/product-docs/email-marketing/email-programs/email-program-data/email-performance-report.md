---
unique-page-id: 2359467
description: Rapporto sulle prestazioni delle e-mail - Documenti Marketo - Documentazione del prodotto
title: Rapporto prestazioni e-mail
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 6133a04124d9d4b829d092943753c7bb530dd374
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Rapporto prestazioni e-mail {#email-performance-report}

Per vedere le prestazioni delle e-mail con statistiche quali consegnate, aperte, su cui è stato fatto clic, ecc., crea un rapporto sulle prestazioni delle e-mail.

1. [Crea un report in un programma](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) e seleziona **Prestazioni e-mail** [Tipo di report](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Modifica l&#39;intervallo di tempo del report](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) e fai clic sulla scheda **Report**.
1. Ci sei! Ora esplora il rapporto per vedere come si sono svolti i messaggi e-mail.

   >[!NOTE]
   >
   >Il filtro Data di invio si basa sulla prima data di invio dell’e-mail.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Fai clic sul nome di un’e-mail per aprirla in Anteprima e-mail.

   >[!NOTE]
   >
   >Un rapporto sulle prestazioni dell’e-mail include attività per tutte le persone, incluse quelle che sono state eliminate dopo l’invio dell’e-mail. A volte ti può capitare di voler vedere le attività solo per le persone attive. In tal caso, è necessario filtrare le persone eliminate dal rapporto. Utilizzare la scheda **Elenco avanzato** per [creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) per il report. Se non si applica alcun filtro a un campo specifico, impostare il filtro Indirizzo e-mail su: **non è vuoto**.

   [Selezionare le colonne del report](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) per un report delle prestazioni delle e-mail:

   <table><thead>
<tr>
    <th>Colonna</th>
    <th>Descrizione</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Rifiuto rigido</td>
    <td>L’e-mail è stata rifiutata a causa di una condizione permanente, ad esempio un indirizzo e-mail inesistente.</td>
  </tr>
  <tr>
    <td>Rimbalzo morbido</td>
    <td>L'e-mail è stata rifiutata a causa di una condizione temporanea, ad esempio un server inattivo o una casella in entrata completa.</td>
  </tr>
  <tr>
    <td>In sospeso</td>
    <td>Questo numero viene calcolato sottraendo il numero di e-mail consegnate, non recapitate e non recapitate dal numero totale inviato.</td>
  </tr>
  <tr>
    <td>Collegamento selezionato</td>
    <td>Numero di destinatari e-mail che hanno fatto clic su un collegamento nell’e-mail.</td>
  </tr>
  <tr>
    <td>Annulla l'iscrizione</td>
    <td>Numero di destinatari e-mail che hanno fatto clic sul collegamento Annulla iscrizione nell’e-mail e hanno compilato il modulo.</td>
  </tr>
  <tr>
    <td>Interrotto</td>
    <td>Numero di e-mail che non è stato possibile recapitare e non è stato ricevuto alcun evento di mancato recapito. Un’e-mail viene automaticamente definita Interrotta se non viene ricevuta una risposta entro tre giorni dall’invio dell’e-mail.</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>I collegamenti e gli indirizzi e-mail per l’annullamento dell’abbonamento su cui si fa clic in un’e-mail non verranno registrati in Collegamenti selezionati nel rapporto.

In generale, cerchiamo di usare il buon senso per registrare queste statistiche. Ad esempio, se qualcuno ha fatto clic su un collegamento in un’e-mail, ovviamente ha aperto prima l’e-mail. Seguiamo queste regole specifiche per il rapporto sulle prestazioni delle e-mail:

* **Regola 1**: ogni record di attività e-mail è impostato su uno dei seguenti valori: _Consegnato_, _Rimbalzato_, _Rimbalzato temporaneamente_ o _In sospeso_.

* **Regola 2**: se il record e-mail mostra *Aperto*, viene conteggiato come *Consegnato*.

* **Regola 3**: se il record e-mail mostra _E-mail selezionata_ o _Non iscritto_, viene conteggiato come _Consegnato_ e _Aperto_.

* **Regola 4**: se l&#39;e-mail è _Aperta_, le mancate consegne vengono ignorate. Se l&#39;e-mail non è stata aperta, _Non recapitato_ ha la precedenza su _Non recapitato_ e _Non recapitato_.

* **Regola 5**: se non viene ricevuta alcuna attività e-mail tre giorni dopo l&#39;invio, verrà considerata _Interrotta_.

>[!NOTE]
>
>* Più invii dalla stessa campagna alla stessa persona vengono conteggiati una sola volta.
>
>* Più invii da campagne diverse alla stessa persona vengono conteggiati separatamente.

>[!MORELIKETHIS]
>
>* [Filtrare Assets nei report e-mail per campagne](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md){target="_blank"}
>* [Filtra record eliminati/uniti in un report sulle prestazioni delle e-mail](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-deleted-merged-records-email-performance-report.md){target="_blank"}
>* [Rapporto prestazioni collegamento e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md){target="_blank"}
