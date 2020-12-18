---
unique-page-id: 2950555
description: Modifica impostazioni Facebook Rich Post - Documenti Marketo - Documentazione del prodotto
title: Modifica impostazioni post RTF Facebook
translation-type: tm+mt
source-git-commit: 44ed91b485b52173922c709de63a4353e16c5072
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---


# Modifica impostazioni post RTF di Facebook {#edit-facebook-rich-post-settings}

Personalizzate i post quando le persone [condividono ](http://docs.marketo.com/display/docs/social) su Facebook.

>[!NOTE]
>
>**Disponibilità**
>
>Non tutti i clienti hanno acquistato questa funzionalità. Per informazioni, contattate il rappresentante commerciale.

Le [app per social network](http://docs.marketo.com/display/docs/social) consentono ai lead di condividere le pagine di destinazione con le loro connessioni sui social network come Facebook, Twitter, ecc. I tag OpenGraph di Facebook (tag OG) consentono di specificare quali informazioni della pagina di destinazione sono incluse nei post di Facebook.

## Seleziona le opzioni per i post avanzati {#select-rich-post-options}

Potete specificare i tipi di informazioni di pagina da utilizzare nei post ricchi di Facebook generati dalle condivisioni dalla pagina di destinazione.

1. Selezionate **Facebook Message** nell&#39;editor per il pulsante video o social di **YouTube**.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Selezionate una delle seguenti opzioni per il messaggio di Facebook.

   * Aggiungi contenuto statico: Selezionate questa opzione per immettere manualmente il titolo, la didascalia e la descrizione.

      ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Aggiungi contenuto dinamico: L&#39;app per social network può utilizzare i tag `<TITLE>`, `<CAPTION>` e `<DESCRIPTION>` della pagina di destinazione per compilare il post RTF.

      ![](assets/image2014-9-22-16-3a48-3a9.png)
   >[!NOTE]
   >
   >Questi dovrebbero già esistere nell&#39;origine della pagina, ma per un maggiore controllo, è possibile [aggiungere specifici tag OG di Facebook alla pagina di destinazione](edit-facebook-rich-post-settings.md).

   * Non aggiungere contenuti avanzati: Limita i post di Facebook dalla pagina di destinazione al messaggio e al collegamento principali.

      ![](assets/image2014-9-22-16-3a48-3a18.png)



## Aggiungere tag OG di Facebook a una pagina di destinazione {#add-facebook-og-tags-to-a-landing-page}

Per controllare gli elementi della pagina che verranno inclusi nelle condivisioni Facebook dalla pagina di destinazione, potete aggiungere alla pagina di destinazione tag OG (Open Graph) di Facebook per titolo, didascalia e descrizione.

1. Aprite la pagina di destinazione che contiene il **pulsante video di YouTube** o il pulsante per social network.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   La **pagina di destinazione Designer** si apre in una nuova finestra.

1. Selezionare **Azioni pagina di destinazione** > **Modifica tag metadati pagina***.**

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Aggiungete l’HTML che definisce og:title, og:caption e og:description. Copiate e incollate queste righe e sostituite il testo segnaposto:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Prestate attenzione a utilizzare la sintassi HTML corretta quando aggiungete i tag OG.
