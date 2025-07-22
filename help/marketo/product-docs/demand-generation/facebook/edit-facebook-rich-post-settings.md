---
unique-page-id: 2950555
description: Modifica le impostazioni dei post avanzati di Facebook - Documentazione di Marketo - Documentazione del prodotto
title: Modifica impostazioni post Rich di Facebook
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
hide: true
hidefromtoc: true
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Modifica impostazioni post formattato [!DNL Facebook] {#edit-facebook-rich-post-settings}

Personalizza i post quando le persone ti condividono su [!DNL Facebook].

>[!AVAILABILITY]
>
>Non tutti gli utenti di Marketo Engage hanno acquistato questa funzionalità. Per informazioni, contatta il team dell’account di Adobe (il tuo Account Manager).

Le _app social_ di Marketo consentono ai lead di condividere le pagine di destinazione con le relative connessioni sui social network, ad esempio Facebook, Twitter e così via. I tag di Facebook OpenGraph (tag OG) consentono di specificare quali informazioni dalla pagina di destinazione vengono incluse nei post di Facebook.

## Seleziona opzioni post formattato {#select-rich-post-options}

Puoi specificare i tipi di informazioni sulla pagina da utilizzare nei [!DNL Facebook] post avanzati generati da condivisioni dalla pagina di destinazione.

1. Seleziona **[!UICONTROL Facebook Message]** nell&#39;editor per il tuo **[!DNL YouTube*]* video o pulsante social.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Selezionare una delle opzioni seguenti per il messaggio [!DNL Facebook].

   * Aggiungi contenuto statico: seleziona questa opzione per inserire manualmente il titolo, la didascalia e la descrizione.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Aggiungi contenuto dinamico: l&#39;app social può utilizzare i tag `<TITLE>`, `<CAPTION>` e `<DESCRIPTION>` della pagina di destinazione per compilare il post RTF.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Questi dovrebbero già esistere nell&#39;origine della pagina, ma per un maggiore controllo, puoi aggiungere specifici tag OG [!DNL Facebook] alla pagina di destinazione.

   * Non aggiungere contenuti avanzati: limita i [!DNL Facebook] post dalla pagina di destinazione al solo messaggio principale e collegamento.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Aggiungi [!DNL Facebook] tag OG a una pagina di destinazione {#add-facebook-og-tags-to-a-landing-page}

Per controllare gli elementi della pagina che verranno inclusi nelle condivisioni [!DNL Facebook] dalla pagina di destinazione, è possibile aggiungere [!DNL Facebook] tag OG (Open Graph) per titolo, didascalia e descrizione alla pagina di destinazione.

1. Apri la pagina di destinazione contenente il tuo **[!DNL YouTube]video** o pulsante per social network.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   **[!UICONTROL Landing Page Designer]** si apre in una nuova finestra.

1. Selezionare **[!UICONTROL Landing Page Actions]** > **[!UICONTROL Edit Page Meta Tags]**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Aggiungere il HTML che definisce og:title, og:caption e og:description. Copiare e incollare queste righe e sostituire il testo segnaposto:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Fai attenzione a utilizzare la sintassi HTML corretta quando aggiungi i tag OG.
