---
unique-page-id: 6094879
description: Aggiunta di un URL target a una campagna web - Documentazione di Marketo - Documentazione del prodotto
title: Aggiunta di un URL di destinazione a una campagna web
exl-id: 5fbb3f12-1474-46c3-8315-8d081422e154
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 9%

---

# Aggiunta di un URL di destinazione a una campagna web {#adding-a-target-url-to-a-web-campaign}

Un URL di Target si trova nella pagina Imposta campagna e definisce l’URL o gli URL specifici in cui verrà visualizzata una campagna web.

## Aggiunta di un URL di destinazione per le campagne Web di finestre di dialogo o widget {#adding-a-target-url-for-dialog-or-widget-web-campaigns}

1. Vai a **[!UICONTROL Web Campaigns]**.

   ![](assets/web-campaigns-hand-5.jpg)

1. Seleziona **[!UICONTROL Create New Web Campaign]**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. Aggiungi **[!UICONTROL Campaign Name]**. Seleziona **[!UICONTROL Target Segment]**. Aggiungi **[!UICONTROL Target URL]**.

   ![](assets/set-web-campaign-hands.jpg)

<table>
 <thead>
  <tr>
   <th colspan="1" rowspan="1">Nome</th>
   <th colspan="1" rowspan="1">Descrizione</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td colspan="1" rowspan="1"><strong>[!UICONTROL Any Page]</strong></td>
   <td colspan="1" rowspan="1"><p>Consenti la visualizzazione della campagna su qualsiasi pagina.</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>[!UICONTROL Include URL parameter when matching]</strong></p></td>
   <td colspan="1" rowspan="1">Aggiungi il parametro URL per far corrispondere e mostrare la campagna sugli URL che includono questo parametro. Esempio: campaign=cpc</td>
  </tr>
 </tbody>
</table>

## Aggiunta di più URL all’URL di destinazione {#adding-multiple-urls-to-target-url}

Facendo clic sull&#39;icona più (![—](assets/image2015-2-18-8-3a40-3a59.png)) verrà aperta la finestra di dialogo [!UICONTROL Multiple Value Entry] per aggiungere più URL. Aggiungi un URL per riga.

![](assets/image2015-2-23-18-3a15-3a57.png)

>[!NOTE]
>
>* Le campagne Web Dialog e Widget possono utilizzare le opzioni Qualsiasi pagina e Carattere jolly (&#42;).
>* Nei casi di utilizzo avanzati, le campagne Web In Zone possono utilizzare caratteri jolly alla fine del percorso URL. Esempio: [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)
>* L’URL distingue tra maiuscole e minuscole

## Aggiunta di un URL di destinazione per le campagne web nell’area {#adding-a-target-url-for-in-zone-web-campaigns}

1. Vai a **[!UICONTROL Web Campaigns]**.

   ![](assets/web-campaigns-hand-5.jpg)

1. Seleziona **[!UICONTROL Create New Web Campaign]**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. Aggiungi **[!UICONTROL Campaign Name]**. Seleziona **[!UICONTROL Target Segment]**. Aggiungi **[!UICONTROL Target URL]**.

   >[!NOTE]
   >
   >L’URL di destinazione con nelle zone deve definire uno o più URL specifici. Nei casi di utilizzo avanzati, le campagne Web In Zone possono utilizzare caratteri jolly alla fine del percorso URL. Esempio: [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)

   ![](assets/set-web-campaign-multiple-hands.jpg)

>[!MORELIKETHIS]
>
>* [Crea una campagna di dialogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [Crea un RTP in una campagna zona](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [Crea una campagna widget RTP](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
