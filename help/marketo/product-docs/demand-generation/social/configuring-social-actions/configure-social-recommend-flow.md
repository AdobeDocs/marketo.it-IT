---
unique-page-id: 2950549
description: Configurare il flusso di consigli per social network - Documentazione di Marketo - Documentazione del prodotto
title: Configura flusso consigli social
exl-id: 01b54215-4a0c-4639-80d2-ec30603b3695
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Configura flusso consigli social {#configure-social-recommend-flow}

Quando crei un’app social, puoi configurare le scelte del social network e i prompt che un utente incontra durante la registrazione.

>[!IMPORTANT]
>
>Il 31 luglio 2024 è iniziato il processo di rimozione di questa funzione. Non è più possibile creare nuove risorse. Le risorse esistenti continueranno a funzionare fino al 31 gennaio 2025. [Ulteriori informazioni](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## Seleziona reti da condividere {#select-networks-for-sharing}

>[!NOTE]
>
>È molto simile a [configurare il flusso di abbonamento/condivisione per social network](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-social-sign-up-share-flow.md), ma si tratta dei collegamenti di condivisione _sotto_ dell&#39;app social.

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Seleziona l&#39;app e fai clic su **Modifica bozza**.

   ![](assets/image2014-9-22-11-3a51-3a6.png)

1. Nell&#39;editor dell&#39;app social, vai a **Flusso consigliato** > **Social network**.

   ![](assets/recommendedflow.png)

1. Selezionare le reti a cui un utente può condividere.

   ![](assets/socialnetworkschoose.png)

## Configurare il messaggio di Facebook {#configure-the-facebook-message}

1. Configura il messaggio che verrà visualizzato nei post di Facebook.

   ![](assets/image2014-9-22-11-3a53-3a21.png)

   >[!NOTE]
   >
   >In una condivisione video, la miniatura viene generata automaticamente.

   Se si sceglie **Aggiungi contenuto dinamico**, i valori dei tag OpenGraph della pagina (og:title, og:caption e og:description) e la miniatura vengono aggiunti automaticamente ai post di Facebook. Vedere il passaggio successivo.

   Se si sceglie **Aggiungi contenuto statico**, immettere il titolo, la didascalia e la descrizione, quindi caricare un&#39;immagine. Consulta i due passaggi successivi.

1. Nella finestra Visualizza e modifica fare clic su **Mostra modifiche** per personalizzare il prompt di condivisione e il messaggio che verranno visualizzati nei post di Facebook.

   >[!TIP]
   >
   >Per ulteriori informazioni, vedere [Modifica impostazioni post RTF di Facebook](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md).

   ![](assets/image2014-9-22-11-3a54-3a36.png)

   >[!NOTE]
   >
   >L&#39;[URL di condivisione](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) viene aggiunto automaticamente a tutti i messaggi di condivisione.

1. Se hai scelto **Aggiungi contenuto statico**, modifica il titolo, la didascalia e la descrizione e carica un&#39;immagine personalizzata (dalle immagini e dai file Marketo).

   ![](assets/image2014-9-22-11-3a55-3a14.png)

   Vedere [Aggiungere immagini e file a Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Se carichi un’immagine, non la visualizzerai qui finché non chiudi e riapri l’editor dell’app social.

1. Fai clic su **Avanti**.

Se selezioni , i valori dei tag OpenGraph della pagina (og:title, og:caption e og:description) e la miniatura vengono aggiunti automaticamente ai post di Facebook. Vedere il passaggio successivo.

## Configurare il messaggio di Twitter {#configure-the-twitter-message}

1. Fare clic per modificare il prompt di condivisione e il messaggio che verranno visualizzati nei tweet di Twitter.

   ![](assets/image2014-9-22-12-3a2-3a40.png)

   >[!TIP]
   >
   >Utilizza {html_title} nel testo del tweet per visualizzare automaticamente il titolo della pagina.

1. Fai clic su **Avanti**.

## Configurare il messaggio di LinkedIn {#configure-the-linkedin-message}

1. Configura il messaggio che verrà visualizzato nei post di LinkedIn.

   ![](assets/image2014-9-22-12-3a3-3a21.png)

   Se si sceglie **Aggiungi contenuto dinamico**, i valori dei tag delle pagine (titolo e descrizione) e della miniatura vengono aggiunti automaticamente ai post di LinkedIn. Vedere il passaggio successivo.

   Se scegli **Aggiungi contenuto statico**, immetti il titolo, la didascalia e la descrizione, quindi carica un&#39;immagine. Consulta i due passaggi successivi.

1. Nella finestra **Visualizza e modifica**, fai clic su **Mostra modifiche** e modifica il prompt di condivisione e il messaggio che verranno visualizzati nei post di LinkedIn.

   ![](assets/image2014-9-22-12-3a3-3a38.png)

   >[!TIP]
   >
   >Utilizza {html_title} nel testo del post per visualizzare automaticamente il titolo della pagina.

1. Se hai scelto **Aggiungi contenuto statico** qui sopra, modifica il titolo e la descrizione e carica un&#39;immagine personalizzata (dalle immagini e dai file Marketo).

   ![](assets/image2014-9-22-12-3a4-3a43.png)

   Vedere [Aggiungere immagini e file a Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Se carichi un’immagine, non la visualizzerai qui finché non chiudi e riapri l’editor dell’app social.

1. Fai clic su **Avanti**.

## Configurare il messaggio di conferma {#configure-the-confirmation-message}

1. Modifica il testo della conferma della condivisione.

   ![](assets/image2014-9-22-12-3a5-3a30.png)

1. Fai clic su **Fine** > **Approva** e **Chiudi**.

   ![](assets/image2014-9-22-12-3a5-3a45.png)

>[!MORELIKETHIS]
>
>Il passaggio successivo è quello di [aggiungere la condivisione video](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-video-share-flow.md) o [sondaggio](/help/marketo/product-docs/demand-generation/social/creating-a-poll/create-a-poll.md) a una pagina di destinazione, a Facebook o al tuo sito Web.
