---
unique-page-id: 1146997
description: Utilizzare un token di data in un passaggio del flusso di attesa - Documenti Marketo - Documentazione del prodotto
title: Utilizzare un token di data in un passaggio di flusso di attesa
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Utilizzare un token di data in un passaggio di flusso di attesa {#use-a-date-token-in-a-wait-flow-step}

Potete utilizzare il passaggio del flusso di attesa per mettere in pausa il viaggio di una persona attraverso una campagna intelligente fino a una data specifica che utilizza un token di data. È inoltre possibile modificare la data di fine di un certo numero di giorni.

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

>[!NOTE]
>
>Ciò vale solo per attivare le campagne. Non è possibile utilizzare questa funzione nelle campagne batch.

1. Nella scheda **Flusso** campagna intelligente, trascina il passaggio del flusso di **attesa** .

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Fate clic sull&#39;icona dell&#39;ingranaggio a destra.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. Dall&#39;elenco a discesa **Tipo** , selezionate Token **** data.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Scegliete un token di data per specificare la fine del passaggio di attesa:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Selezionare la casella per attendere fino al prossimo anniversario della data che si verifica nell&#39;anno civile corrente o successivo.

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Utilizzate questa opzione sui token data che fanno riferimento a date passate, ad esempio una data di compleanno o di inizio contratto.

1. Facoltativamente, puoi modificare la data di fine per un numero specificato di giorni.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >È inoltre possibile specificare il numero di giorni utilizzando un `{{lead.` token o un `{{company.` campo intero o un `{{my.` token di tipo numerico.

1. Fate clic su Salva.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!NOTE]
   >
   >**Articoli correlati**
   >
   >* [Utilizzo di una durata in un passaggio del flusso di attesa](use-a-duration-in-a-wait-flow-step.md)
   >* [Utilizzare una data specifica in un passaggio del flusso di attesa](use-a-specific-date-in-a-wait-flow-step.md)


