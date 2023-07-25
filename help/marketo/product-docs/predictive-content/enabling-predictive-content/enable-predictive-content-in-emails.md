---
unique-page-id: 11385020
description: Abilitare il contenuto predittivo nelle e-mail - Documenti Marketo - Documentazione del prodotto
title: Abilitare il contenuto predittivo nelle e-mail
exl-id: 7eaefee1-23e8-47ee-afff-adcf49096aa7
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '387'
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
>* **Preparare i contenuti predittivi**
>
>   * [Modifica contenuto predittivo per le e-mail](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target="_blank"} o
>   * [Modifica contenuto predittivo per contenuti rich media](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target="_blank"} o
>   * [Modifica contenuto predittivo per la barra dei consigli](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target="_blank"}
>
>* [Approvare un titolo per il contenuto predittivo](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target="_blank"}

## Aggiunta di contenuto predittivo tramite l’editor di e-mail 2.0 {#adding-predictive-content-using-the-email-editor}

1. Clic **Attività di marketing**.

   ![](assets/one.png)

1. Seleziona l’e-mail e fai clic su **Modifica bozza**.

   ![](assets/two.png)

1. Fai clic sull’immagine da rendere predittiva. Quando viene visualizzata l’icona a forma di ingranaggio, fai clic su di essa e seleziona **Abilita ContentAI** (ContentAI è il nome precedente di Predictive Content).

   ![](assets/three.png)

1. Per selezionare una o più categorie, fare clic sul pulsante **Categorie** , effettuare le selezioni e fare clic su **Applica**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >La scelta di categorie specifiche o la modifica del layout predittivo è facoltativa.

1. L&#39;immagine è ora predittiva. Ripetere i punti 3 e 4 per ulteriori immagini (se si desidera).

   ![](assets/five.png)

1. Per visualizzare l’anteprima del messaggio e-mail, fai clic su **Anteprima** nell’angolo superiore destro.

   ![](assets/six.png)

1. Per visualizzare diverse immagini possibili, fai clic su **Aggiorna**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Immagine non selezionata **_fino a quando il destinatario non apre l’e-mail_**. Quindi quello che vedi nell&#39;anteprima è solo un esempio, e non sarà necessariamente l&#39;immagine che vede il destinatario.

1. Dopo aver visualizzato l’anteprima del messaggio e-mail, fai clic su **Anteprima azioni** a discesa e selezionare **Approva e chiudi**. In alternativa, se è ancora necessario apportare modifiche, fare clic su **Modifica bozza** a destra.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Quando si invia un campione, viene selezionata un’immagine casuale.

Dopo che avrai approvato l’e-mail, questa sarà dotata di Contenuto predittivo e pronta per l’invio.

>[!CAUTION]
>
>Una volta che un destinatario apre l’e-mail, le immagini predittive vengono bloccate. Se il contenuto viene successivamente rimosso, i destinatari visualizzeranno un’immagine interrotta in cui si trovava il contenuto.

## Aggiunta di contenuto predittivo quando non si utilizza l’editor di e-mail 2.0 {#adding-predictive-content-when-not-using-the-email-editor}

Se non utilizzi un’ [E-mail 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md){target="_blank"} modello, l’aggiunta di Contenuto predittivo all’e-mail può essere eseguita semplicemente assegnando un tag a un’immagine nel modello come elemento immagine modificabile di Marketo.

Scopri di più su [Sintassi specifica per Marketo](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements){target="_blank"}.

Di seguito è riportato un esempio dell’aspetto del codice (questo è solo un esempio, non copiare esattamente il codice seguente).

**Esempio**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
