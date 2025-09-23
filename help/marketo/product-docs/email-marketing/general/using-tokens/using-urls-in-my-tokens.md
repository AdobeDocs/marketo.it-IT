---
unique-page-id: 11382535
description: 'Utilizzo degli URL nei token: documenti Marketo: documentazione del prodotto'
title: Utilizzo degli URL nei miei token
exl-id: 6830c621-4d94-4f31-a608-2f7b2aced88c
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 5%

---

# Utilizzo degli URL nei miei token {#using-urls-in-my-tokens}

Segui i passaggi seguenti per utilizzare [!UICONTROL My Tokens] per inserire gli URL nelle e-mail.

1. Selezionare il programma e fare clic su **[!UICONTROL My Tokens]**.

   ![](assets/one-4.png)

1. Seleziona il token **[!UICONTROL Text]**, trascinalo sull&#39;area di lavoro.

   ![](assets/two-4.png)

1. Assegna al token un nome univoco, immetti un URL (senza https://) e fai clic su **[!UICONTROL Save]**.

   ![](assets/three-4.png)

   >[!CAUTION]
   >
   >**Utilizzo di http/https...**
   >
   >* Per assicurarti che i clic siano tracciati nel messaggio e-mail, **non** immetti https:// _all&#39;interno_ del valore del token. Utilizzalo all’esterno del token, come illustrato nel passaggio 7.
   >
   >* Si consiglia vivamente di non escludere il http/https. Così facendo, la [versione web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} dell&#39;e-mail potrebbe essere riprodotta in modo errato.

1. Seleziona l’e-mail nel programma.

   ![](assets/four-3.png)

1. Fai clic su **[!UICONTROL Edit Draft]**.

   ![](assets/five-3.png)

1. Fare doppio clic nell&#39;area di testo da modificare.

   ![](assets/six-1.png)

1. In qualsiasi punto dell&#39;e-mail, digita `https://` (senza lasciare spazio dopo) e fai clic sull&#39;icona Inserisci token.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Naturalmente puoi anche immettere `http://` se il tuo sito non utilizza https.

1. Individua il token personale, selezionalo e fai clic su **[!UICONTROL Insert]**.

   ![](assets/eight.png)

1. Evidenziare https:// e il token, quindi premere Ctrl/Comando+X (Ctrl = Windows/Comando = Mac) per tagliare il testo.

   ![](assets/nine.png)

1. Evidenziare il testo da visualizzare nel collegamento e fare clic sull&#39;icona [!UICONTROL Insert/Edit Link].

   ![](assets/ten.png)

1. Premere Ctrl/Comando+V per incollare il contenuto nella casella **[!UICONTROL URL]** e fare clic su **[!UICONTROL Insert]**.

   ![](assets/eleven.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/twelve.png)

   E hai finito! L’URL si popolerà dopo l’invio e, grazie al fatto che inserisci https:// davanti al token, genererà un collegamento tracciabile.
