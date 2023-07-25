---
unique-page-id: 7504676
description: Informazioni sui costi dei periodi - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sui costi del periodo
exl-id: 99f50eaf-28cf-4a8b-8ebd-89a4beef986a
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Informazioni sui costi del periodo {#understanding-period-costs}

## Panoramica {#overview}

I costi del periodo si riferiscono al denaro speso in un mese specifico per un programma.

>[!NOTE]
>
>**Esempio**
>
>Se si spendono $ 1000 per assumere un illustratore per un eBook che viene lanciato a luglio, il programma eBook avrebbe un costo di periodo di $ 1000 a luglio.
>
>Se spendi 200 dollari al mese in Google Adwords, il programma Google Adwords avrà un costo di periodo di 200 dollari **ogni mese**.

>[!NOTE]
>
>[Informazioni sui programmi](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Informazioni sull’iscrizione al programma](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## Modalità di calcolo dei costi del periodo {#how-period-costs-are-calculated}

Immaginate un evento, come un webinar, che si verifica a marzo. Le nuove persone vengono acquisite in anticipo dalla pubblicità nei mesi di gennaio e febbraio. Nuovi contatti vengono acquisiti anche dopo l&#39;evento, quando le persone scaricano il webinar nei mesi di aprile e maggio.

1. Con un solo periodo di costo attribuito a marzo...

   ![](assets/graph1.png)

   ...contatti aggiunti nei mesi precedenti e successivi verranno *solo* contare verso marzo.

   ![](assets/graph2.png)

1. Con i costi del periodo attribuiti a gennaio, febbraio e marzo...

   ![](assets/graph3.png)

   ...i contatti aggiunti solo nei mesi successivi a marzo saranno conteggiati verso marzo.

   ![](assets/graph4.png)

1. Con i costi del periodo attribuiti a gennaio e aprile...

   ![](assets/graph5.png)

   ...i contatti aggiunti nei mesi da gennaio a marzo saranno conteggiati per gennaio. I contatti aggiunti nei mesi di aprile e maggio saranno conteggiati per aprile.

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >In sintesi: se per un mese non è definito alcun periodo, i costi verranno riportati all&#39;ultimo periodo definito. Se non è presente alcun costo del periodo precedente, i mesi verranno riportati &quot;in avanti&quot; al successivo periodo definito. Se non è stato definito un costo di periodo per _qualsiasi_ mesi, il reporting in RCE non sarà disponibile per il programma.

   >[!MORELIKETHIS]
   >
   >* [Utilizzo dei costi del periodo in un programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [Filtrare un rapporto Programma per costo periodo](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)
