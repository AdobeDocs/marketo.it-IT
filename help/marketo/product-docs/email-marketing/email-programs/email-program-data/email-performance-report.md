---
unique-page-id: 2359467
description: Rapporto sulle prestazioni delle e-mail - Documenti Marketo - Documentazione del prodotto
title: Rapporto prestazioni e-mail
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '428'
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

   | Colonna | Descrizione |
   |---|---|
   | Rifiuto rigido | L’e-mail è stata rifiutata a causa di una condizione permanente, ad esempio un indirizzo e-mail inesistente. |
   | Rimbalzo morbido | L&#39;e-mail è stata rifiutata a causa di una condizione temporanea, ad esempio un server inattivo o una casella in entrata completa. |
   | In sospeso | Questo numero viene calcolato sottraendo il numero di e-mail consegnate, non recapitate e non recapitate dal numero totale inviato. |
   | Collegamento selezionato | Numero di destinatari e-mail che hanno fatto clic su un collegamento nell’e-mail. |
   | Annulla l&#39;iscrizione | Numero di destinatari e-mail che hanno fatto clic sul collegamento **Annulla iscrizione** nell&#39;e-mail e hanno compilato il modulo. |

   >[!NOTE]
   >
   >I collegamenti e gli indirizzi e-mail per l’annullamento dell’abbonamento su cui si fa clic in un’e-mail non verranno registrati in Collegamenti selezionati nel rapporto.

In generale, cerchiamo di usare il buon senso per registrare queste statistiche. Ad esempio, se qualcuno ha fatto clic su un collegamento in un’e-mail, ovviamente ha aperto prima l’e-mail. Seguiamo queste regole specifiche per il rapporto sulle prestazioni delle e-mail:

* **Regola 1**: ogni record di attività e-mail è impostato su uno dei seguenti valori: _Consegnato_, _Rimbalzato_, _Rimbalzato temporaneamente_ o _In sospeso_.

* **Regola 2**: se il record e-mail mostra *Aperto*, viene conteggiato come *Consegnato*.

* **Regola 3**: se il record e-mail mostra _E-mail selezionata_ o _Non iscritto_, viene conteggiato come _Consegnato_ e _Aperto_.

* **Regola 4**: se l&#39;e-mail è _Aperta_, le mancate consegne vengono ignorate. Se l&#39;e-mail non è stata aperta, _Non recapitato_ ha la precedenza su _Non recapitato_ e _Non recapitato_.

>[!NOTE]
>
>Più invii dalla stessa campagna alla stessa persona vengono conteggiati una sola volta.

>[!MORELIKETHIS]
>
>* [Filtrare Assets nei report e-mail per campagne](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Rapporto prestazioni collegamento e-mail](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)
