---
unique-page-id: 11385020
description: Abilita contenuto predittivo nelle e-mail - Documenti Marketo - Documentazione del prodotto
title: Abilitare il contenuto predittivo nelle e-mail
exl-id: 7eaefee1-23e8-47ee-afff-adcf49096aa7
source-git-commit: 4b1b91a933a7a6d103fe0d44ece9ea95759edc5f
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Abilitare il contenuto predittivo nelle e-mail {#enable-predictive-content-in-emails}

Rendi predittiva una o più immagini nell’e-mail, adattando l’esperienza per ogni destinatario.

>[!NOTE]
>
>Si consiglia di abilitare più di cinque contenuti per categoria e per fonte (e-mail, rich media, barra) prima di testare e utilizzare il contenuto predittivo. Più contenuto ti dà un risultato predittivo migliore.

>[!PREREQUISITES]
>
>Prima di abilitare il contenuto predittivo, devi:
>
>* **Preparare il contenuto predittivo**
   >
   >   * [Modifica del contenuto predittivo per le e-mail](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target=&quot;_blank&quot;} o
   >   * [Modifica di contenuti predittivi per contenuti rich media](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target=&quot;_blank&quot;} o
   >   * [Modifica contenuto predittivo per la barra delle raccomandazioni](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target=&quot;_blank&quot;}
>
>* [Approvare un titolo per il contenuto predittivo](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target=&quot;_blank&quot;}


## Aggiunta di contenuti predittivi tramite l’editor di e-mail 2.0 {#adding-predictive-content-using-the-email-editor}

1. Fai clic su **Attività di marketing**.

   ![](assets/one.png)

1. Seleziona l’e-mail e fai clic su **Modifica bozza**.

   ![](assets/two.png)

1. Fai clic sull’immagine da rendere predittiva. Quando viene visualizzata l’icona a forma di ingranaggio, fai clic su di essa e seleziona **Abilita ContentAI** (ContentAI è il nome precedente per Predictive Content (Contenuto predittivo).

   ![](assets/three.png)

1. Per selezionare una o più categorie, fai clic sul pulsante **Categorie** effettua le selezioni e fai clic su **Applica**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >La scelta di categorie specifiche o la modifica del layout predittivo è facoltativa.

1. L&#39;immagine è ora predittiva. Ripetere i passaggi 3 e 4 per ulteriori immagini (se necessario).

   ![](assets/five.png)

1. Per visualizzare l’anteprima del messaggio e-mail, fai clic su **Anteprima** nell&#39;angolo in alto a destra.

   ![](assets/six.png)

1. Per visualizzare diverse immagini possibili, fai clic su **Aggiorna**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >L’immagine non è selezionata **_fino a quando il destinatario non apre l’e-mail_**. Quello che vedete nell&#39;anteprima è solo un esempio, e non sarà necessariamente l&#39;immagine che il destinatario vede.

1. Dopo aver visualizzato l’anteprima del messaggio e-mail, fai clic sul pulsante **Anteprima azioni** a discesa e seleziona **Approva e chiudi**. Oppure, se hai ancora modifiche da fare, fai clic su **Modifica bozza** a destra.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Quando si invia un campione, viene selezionata un’immagine casuale.

Dopo aver approvato l’e-mail, questa sarà dotata di Predictive Content e sarà pronta per l’invio!

>[!CAUTION]
>
>Una volta che un destinatario apre l’e-mail, le immagini predittive vengono bloccate. Se il contenuto viene successivamente rimosso, i destinatari vedranno un’immagine non funzionante in cui si trovava il contenuto.

## Aggiunta di contenuto predittivo quando non si utilizza l’editor di e-mail 2.0 {#adding-predictive-content-when-not-using-the-email-editor}

Se non utilizzi un [Email 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)Il modello {target=&quot;_blank&quot;}, per aggiungere contenuto predittivo all’e-mail, è sufficiente assegnare tag a un’immagine nel modello come elemento immagine modificabile Marketo.

Scopri le [Sintassi specifica di Marketo](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements){target=&quot;_blank&quot;}.

Ecco un esempio di come dovrebbe essere il codice (questo è solo un esempio, non copiare esattamente il codice sottostante).

**Esempio**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
