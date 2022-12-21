---
unique-page-id: 2359467
description: Rapporto sulle prestazioni delle e-mail - Documenti Marketo - Documentazione del prodotto
title: Rapporto prestazioni e-mail
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Rapporto prestazioni e-mail {#email-performance-report}

Per verificare le prestazioni delle e-mail con statistiche come consegnate, aperte, su cui hai fatto clic, ecc., crea un rapporto sulle prestazioni delle e-mail.

1. [Creare un rapporto in un programma](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) e seleziona la **Prestazioni e-mail** [Tipo di rapporto](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Modificare l’intervallo di tempo del rapporto](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) e fai clic su **Rapporto** scheda .
1. Ci sei! Ora esplora il rapporto per vedere le prestazioni delle e-mail.

   >[!NOTE]
   >
   >Il filtro Data di invio si basa sulla prima data di invio dell’e-mail.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Fai clic sul nome di un messaggio e-mail per aprirlo nel visualizzatore e-mail di anteprima.

   >[!NOTE]
   >
   >Un rapporto sulle prestazioni dell’e-mail include attività per tutte le persone, comprese quelle che sono state eliminate dall’invio dell’e-mail. A volte, desideri visualizzare le attività solo per le persone attive. In tal caso, devi filtrare le persone eliminate dal rapporto. Utilizza la **Elenco avanzato** scheda a [creare un elenco smart](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) per la relazione. Se non stai filtrando su un campo specifico, imposta il filtro Indirizzo e-mail su: **non è vuoto**.

   [Seleziona colonne rapporto](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) per un rapporto sulle prestazioni di e-mail:

   | Colonna | Descrizione |
   |---|---|
   | duro rimbalzato | L&#39;e-mail è stata rifiutata a causa di una condizione permanente, ad esempio un indirizzo e-mail inesistente. |
   | Soft rimbalzato | L&#39;e-mail è stata rifiutata a causa di una condizione temporanea, ad esempio un server inattivo o una casella in entrata completa. |
   | In sospeso | Questo numero viene calcolato sottraendo il numero di e-mail inviate, rimbalzate e rimbalzate rispetto al numero totale inviato. |
   | Collegamento selezionato | Numero di destinatari e-mail che hanno fatto clic su un collegamento nell’e-mail. |
   | Annulla l&#39;iscrizione | Numero di destinatari e-mail che hanno fatto clic sul pulsante **Annulla sottoscrizione** collegamento nell’e-mail e compilazione del modulo. |

   >[!NOTE]
   >
   >I collegamenti per l’annullamento dell’abbonamento e gli indirizzi e-mail su cui si fa clic in un messaggio e-mail non vengono registrati nel rapporto in Collegamenti selezionati .

In generale, cerchiamo di usare il buon senso per registrare queste statistiche. Ad esempio, se qualcuno ha fatto clic su un collegamento in un’e-mail, ovviamente ha aperto prima l’e-mail. Seguiamo queste regole specifiche per il rapporto Prestazioni e-mail:

* **Articolo 1**: Ogni record di attività e-mail è impostato su uno e solo uno dei seguenti: _Consegnato_, _duro rimbalzato_, _Soft rimbalzato_ oppure _In sospeso_.

* **Articolo 2**: Se viene visualizzato il record e-mail *Aperto*, viene conteggiato come *Consegnato*.

* **Articolo 3**: Se viene visualizzato il record e-mail _E-mail selezionata_ o _Annulla sottoscrizione_, viene conteggiato come _Consegnato_ e _Aperto_.

* **Articolo 4**: Se l’e-mail è _Aperto_, i messaggi non recapitati vengono ignorati. Se l’e-mail non è stata aperta, _duro rimbalzato_ ha la precedenza _Soft rimbalzato_ e _Consegnato_.

>[!NOTE]
>
>Più invii dalla stessa campagna alla stessa persona vengono conteggiati una sola volta.

>[!MORELIKETHIS]
>
>* [Filtrare le risorse nei rapporti e-mail di Campaign](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Rapporto sulle prestazioni dei collegamenti e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)

