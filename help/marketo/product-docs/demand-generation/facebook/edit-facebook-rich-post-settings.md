---
unique-page-id: 2950555
description: Modificare le impostazioni di Facebook Rich Post - Documentazione Marketo - Documentazione del prodotto
title: Modifica impostazioni di Facebook Rich Post
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---

# Modifica impostazioni di Facebook Rich Post {#edit-facebook-rich-post-settings}

Personalizza i post quando le persone ti condividono su Facebook.

>[!AVAILABILITY]
>
>Non tutti i clienti hanno acquistato questa funzionalità. Contatta il tuo rappresentante commerciale per i dettagli.

Marketo [app social](/help/marketo/product-docs/demand-generation/social/social-functions/add-a-social-button-on-a-landing-page.md) consenti ai lead di condividere le pagine di destinazione con le loro connessioni su social network come Facebook, Twitter, ecc. I tag OpenGraph di facebook (tag OG) consentono di specificare quali informazioni della pagina di destinazione sono incluse nei post di Facebook.

## Selezionare le opzioni del post RTF {#select-rich-post-options}

Puoi specificare i tipi di informazioni di pagina da utilizzare nei post rich post di Facebook generati dalle condivisioni dalla pagina di destinazione.

1. Seleziona **Messaggio facebook** nell’editor per **YouTube** pulsante video o social.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Seleziona una delle seguenti opzioni per il messaggio Facebook.

   * Aggiungi contenuto statico: Selezionare questa opzione per immettere manualmente il titolo, la didascalia e la descrizione.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Aggiungi contenuto dinamico: L’app social può utilizzare le’ della pagina di destinazione `<TITLE>`, `<CAPTION>`e `<DESCRIPTION>` tag per popolare il tuo post RTF.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Questi dovrebbero già esistere nell’origine della pagina, ma per un maggiore controllo, puoi aggiungere alla pagina di destinazione tag OG specifici di Facebook.

   * Non aggiungere contenuti avanzati: Limita i post di Facebook dalla pagina di destinazione al solo messaggio principale e al collegamento.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Aggiungere tag OG di Facebook a una pagina di destinazione {#add-facebook-og-tags-to-a-landing-page}

Per controllare gli elementi della pagina che verranno inclusi nelle condivisioni Facebook dalla pagina di destinazione, puoi aggiungere alla pagina di destinazione tag OG (Open Graph) di Facebook per titolo, didascalia e descrizione.

1. Apri la pagina di destinazione che contiene **Video YouTube** o pulsante social.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   La **Progettazione pagine di destinazione** si apre in una nuova finestra.

1. Seleziona **Azioni pagina di destinazione** > **Modifica tag dei metadati di una pagina**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Aggiungi il HTML che definisce og:title, og:caption e og:description. Copiare e incollare queste righe e sostituire il testo segnaposto:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Quando aggiungi i tag OG, assicurati di utilizzare la sintassi HTML corretta.
