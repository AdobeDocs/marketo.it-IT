---
unique-page-id: 11385020
description: Abilitare il contenuto predittivo nelle e-mail - Documenti Marketo - Documentazione del prodotto
title: Abilitare il contenuto predittivo nelle e-mail
exl-id: 7eaefee1-23e8-47ee-afff-adcf49096aa7
feature: Predictive Content
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---

# Abilitare il contenuto predittivo nelle e-mail {#enable-predictive-content-in-emails}

Rendi predittive una o più immagini nell’e-mail, personalizzando l’esperienza per ogni destinatario.

>[!NOTE]
>
>Si consiglia di abilitare oltre cinque contenuti per categoria e per origine (e-mail, rich media, barra) prima di testare e utilizzare Contenuto predittivo. Più contenuti consentono di ottenere risultati predittivi migliori.

>[!PREREQUISITES]
>
>Prima di abilitare il contenuto predittivo, è necessario:
>
>* **Prepara il contenuto predittivo**
>
>   * [Modifica contenuto predittivo per e-mail](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target="_blank"} o
>   * [Modifica contenuto predittivo per contenuti rich media](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target="_blank"} o
>   * [Modifica contenuto predittivo per la barra dei consigli](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target="_blank"}
>
>* [Approva un titolo per il contenuto predittivo](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target="_blank"}

## Aggiunta di contenuto predittivo tramite l’editor di e-mail 2.0 {#adding-predictive-content-using-the-email-editor}

1. Fai clic su **[!UICONTROL Marketing Activities]**.

   ![](assets/one.png)

1. Selezionare l&#39;indirizzo di posta elettronica e fare clic su **[!UICONTROL Edit Draft]**.

   ![](assets/two.png)

1. Fai clic sull’immagine da rendere predittiva. Quando viene visualizzata l&#39;icona a forma di ingranaggio, fare clic su di essa e selezionare **[!UICONTROL Enable ContentAI]** (ContentAI è il nome precedente di Predictive Content).

   ![](assets/three.png)

1. Per selezionare una o più categorie, fare clic sull&#39;elenco a discesa **[!UICONTROL Categories]**, effettuare le selezioni desiderate e fare clic su **[!UICONTROL Apply]**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >La scelta di categorie specifiche o la modifica del layout predittivo è facoltativa.

1. L&#39;immagine è ora predittiva. Ripetere i punti 3 e 4 per ulteriori immagini (se si desidera).

   ![](assets/five.png)

1. Per visualizzare l&#39;anteprima del tuo indirizzo e-mail, fai clic su **[!UICONTROL Preview]** in alto a destra.

   ![](assets/six.png)

1. Per visualizzare diverse immagini possibili, fare clic su **[!UICONTROL Refresh]**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >L&#39;immagine non è selezionata **_finché il destinatario non apre l&#39;e-mail_**. Quindi quello che vedi nell&#39;anteprima è solo un esempio, e non sarà necessariamente l&#39;immagine che vede il destinatario.

1. Dopo aver visualizzato l&#39;anteprima del messaggio di posta elettronica, fare clic sul menu a discesa **[!UICONTROL Preview Actions]** e selezionare **[!UICONTROL Approve and Close]**. Oppure, se hai ancora delle modifiche da fare, fai clic su **[!UICONTROL Edit Draft]** a destra.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Quando si invia un campione, viene selezionata un’immagine casuale.

Dopo che avrai approvato l’e-mail, questa sarà dotata di Contenuto predittivo e pronta per l’invio.

>[!CAUTION]
>
>Una volta che un destinatario apre l’e-mail, le immagini predittive vengono bloccate. Se il contenuto viene successivamente rimosso, i destinatari visualizzeranno un’immagine interrotta in cui si trovava il contenuto.

## Aggiunta di contenuto predittivo quando non si utilizza l’editor di e-mail 2.0 {#adding-predictive-content-when-not-using-the-email-editor}

Se non utilizzi un modello di [E-mail 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md){target="_blank"}, puoi aggiungere contenuto predittivo all&#39;e-mail semplicemente assegnando un tag a un&#39;immagine nel modello come elemento immagine modificabile di Marketo.

Scopri la sintassi specifica di [Marketo qui](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements){target="_blank"}.

Di seguito è riportato un esempio dell’aspetto del codice (questo è solo un esempio, non copiare esattamente il codice seguente).

**Esempio**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
