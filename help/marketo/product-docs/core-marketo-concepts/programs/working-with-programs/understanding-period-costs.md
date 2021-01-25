---
unique-page-id: 7504676
description: Comprendere i costi del periodo - Documenti Marketo - Documentazione del prodotto
title: Informazioni sui costi del periodo
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# Informazioni sui costi del periodo {#understanding-period-costs}

## Panoramica {#overview}

I costi del periodo si riferiscono ai soldi spesi in un mese specifico per un programma.

>[!NOTE]
>
>**Esempio**
>
>Se si spende $1000 per noleggiare un illustratore per un eBook che si avvia in luglio - il programma eBook avrà un costo di periodo di $1000 in luglio.
>
>Se si spende $200 al mese su Google Adwords - il programma Google Adwords avrebbe un costo di periodo di $200 **ogni mese**.

>[!NOTE]
>
>[Informazioni sui programmi](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Informazioni sull&#39;iscrizione al programma](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## Modalità di calcolo dei costi del periodo {#how-period-costs-are-calculated}

Immaginate un evento, come un webinar, che si terrà a marzo. Le nuove persone vengono acquisite in anticipo dalla pubblicità di gennaio e febbraio. Dopo l&#39;evento vengono acquisiti nuovi contatti, quando le persone scaricano il webinar nei mesi di aprile e maggio.

1. Con un unico periodo di costo attribuito a marzo...

   ![](assets/graph1.png)

   ...i contatti aggiunti nei mesi precedenti e successivi saranno conteggiati *solo* verso marzo.

   ![](assets/graph2.png)

1. Con i costi di periodo attribuiti a gennaio, febbraio e marzo...

   ![](assets/graph3.png)

   ...I contatti aggiunti solo nei mesi successivi a marzo saranno conteggiati per marzo.

   ![](assets/graph4.png)

1. Con i costi di periodo attribuiti a gennaio e aprile...

   ![](assets/graph5.png)

   ...I contatti aggiunti nei mesi da gennaio a marzo saranno conteggiati verso gennaio. I contatti aggiunti nei mesi di aprile e maggio saranno conteggiati verso aprile.

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >In sintesi: mesi senza un periodo definito i costi passeranno &quot;indietro&quot; all&#39;ultimo che è stato definito. Se non esiste un costo per il periodo precedente, i mesi verranno &quot;inoltrati&quot; a quello successivo definito. Se il costo del periodo non è stato definito per _qualsiasi_ mesi, la segnalazione in RCE non sarà disponibile per il programma.

   >[!MORELIKETHIS]
   >
   >* [Utilizzo dei costi del periodo in un programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [Filtra un rapporto programma per costo periodo](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)

