---
unique-page-id: 2359807
description: Personalizzare gli stili di Sweepstakes - Documentazione di Marketo - Documentazione del prodotto
title: Personalizzare gli stili di Sweepstakes
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 1%

---

# Personalizzare gli stili di Sweepstakes {#customize-sweepstakes-styles}

Quando [crei una verifica](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), puoi personalizzarne l&#39;aspetto nella pagina di destinazione.

>[!IMPORTANT]
>
>Il 31 luglio 2024 è iniziato il processo di rimozione di questa funzione. Non è più possibile creare nuove risorse. Le risorse esistenti continueranno a funzionare fino al 31 gennaio 2025. [Ulteriori informazioni](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>Non tutti gli utenti del Marketo Engage hanno acquistato questa funzionalità. Per ulteriori informazioni, contatta l’Adobe Account Team (il tuo Account Manager).

1. Vai a **Attività di marketing**.

![](assets/login-marketing-activities-1.png)

1. Selezionare le puntate e fare clic su **Modifica bozza**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. Nell&#39;editor dei file di sweepstakes, vai a **Impostazioni app** > **Aspetto**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Modifica il testo del pulsante di registrazione e il collegamento di avanzamento.

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Per ogni elemento che desideri personalizzare, immetti le proprietà CSS personalizzate.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Esempio di CSS per il **pulsante Invio**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   Immagine di esempio per il **pulsante Invio**:
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Se utilizzi un&#39;immagine con del testo, ricorda di rimuovere il testo dal campo **Pulsante di immissione** sotto Testo qui sopra.

1. Ogni volta che apportate una modifica, il risultato viene visualizzato nell&#39;anteprima Visualizza e modifica.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >Prova il pulsante in diversi browser, incluse le versioni precedenti.

   >[!MORELIKETHIS]
   >
   >Il passaggio successivo consiste nell&#39;aggiungere [e-mail di iscrizione e di evasione alle tue azioni](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
