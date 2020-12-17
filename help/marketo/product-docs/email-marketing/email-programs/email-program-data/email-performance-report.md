---
unique-page-id: 2359467
description: Rapporto sulle prestazioni e-mail - Documenti Marketo - Documentazione prodotto
title: Report prestazioni e-mail
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---


# Report prestazioni e-mail {#email-performance-report}

Per verificare il livello di prestazioni dei messaggi e-mail con stati come consegnati, aperti, su cui è stato fatto clic, ecc., create un report sulle prestazioni dell&#39;e-mail.

1. [Crea un report in un ](../../../../product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) programma e seleziona il tipo **di report** [Email ](../../../../product-docs/reporting/basic-reporting/report-types/report-type-overview.md)PerformanceReport.
1. [Modificate il ](../../../../product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) frame dell&#39;ora del rapporto e fate clic sulla scheda  **** Rapporto.
1. Sei lì! Esplorate il rapporto per vedere come sono state inviate le e-mail.

   >[!NOTE]
   >
   >Il filtro Data di invio si basa sulla prima data di invio del messaggio e-mail.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Fate clic sul nome di un messaggio e-mail per aprirlo nel visualizzatore di anteprima e-mail.

   >[!NOTE]
   >
   >
   >Un rapporto sulle prestazioni dell&#39;e-mail include attività per tutte le persone, comprese quelle che sono state eliminate dall&#39;invio dell&#39;e-mail. A volte, si desidera visualizzare le attività solo per le persone attive. In tal caso, dovete filtrare le persone eliminate dal rapporto. Utilizzate la scheda **Smart List** per [creare un elenco smart](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) per il report. Se non state applicando un filtro su un campo specifico, impostate il filtro Indirizzo e-mail su: **non è vuoto**.

   [Seleziona ](../../../../product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) Colori rapporto per un rapporto Prestazioni e-mail:

   | Colonna | Descrizione |
   |---|---|
   | Bloccato duro | L&#39;e-mail è stata rifiutata a causa di una condizione permanente, ad esempio un indirizzo e-mail inesistente. |
   | Soft Bounce | L&#39;e-mail è stata rifiutata a causa di una condizione temporanea, ad esempio un server inattivo o una inbox completa. |
   | In sospeso | Questo numero viene calcolato sottraendo il numero di e-mail distribuite, rimbalzate e rimbalzate rispetto al numero totale inviato. |
   | Collegamento selezionato | Numero di destinatari e-mail che hanno fatto clic su un collegamento nell’e-mail. |
   | Annulla sottoscrizione | Numero di destinatari e-mail che hanno fatto clic sul collegamento **Annulla sottoscrizione** nell&#39;e-mail e hanno compilato il modulo. |

   >[!NOTE]
   >
   >I collegamenti per l’annullamento della sottoscrizione e gli indirizzi e-mail su cui si fa clic in un messaggio e-mail non vengono registrati in Collegamenti selezionati nel rapporto.

In generale, cerchiamo di usare il buon senso per registrare queste statistiche. Ad esempio, se qualcuno ha fatto clic su un collegamento in un&#39;e-mail, ovviamente ha aperto prima l&#39;e-mail. Seguiamo queste regole specifiche per il report sulle prestazioni delle e-mail:

* **Articolo 1**: Ogni record di attività e-mail è impostato su uno e solo uno dei seguenti:  *Consegnato*,  *Bloccato* duro,  *Soft Bounced* o  *In sospeso*.

* **Articolo 2**: Se il record e-mail è  *Aperto*, viene conteggiato come  *Consegnato*.

* **Articolo 3**: Se il record e-mail mostra  *Messaggio* e-mail selezionato  *Non iscritto*, viene conteggiato come  ** Consegna e  *Aperto*.

* **Articolo 4**: Se l’e-mail viene  *aperta*, i rimbalzi vengono ignorati. Se l&#39;e-mail non è stata aperta, *Hard Bounced* ha la precedenza su *Soft Bounced* e *Delivery*.

>[!NOTE]
>
>Più invii dalla stessa campagna alla stessa persona vengono conteggiati solo una volta.

>[!MORELIKETHIS]
>
>* [Filtrare le risorse nei rapporti e-mail della campagna](../../../../product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Report prestazioni collegamento e-mail](email-link-performance-report.md)

>



>[!NOTE]
>
>**Tubo profondo**
>
>Ulteriori informazioni in [Base Reporting](http://docs.marketo.com/display/docs/basic+reporting).

