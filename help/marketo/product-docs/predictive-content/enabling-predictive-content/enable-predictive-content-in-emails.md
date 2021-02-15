---
unique-page-id: 11385020
description: Abilita contenuto predittivo nelle e-mail - Documenti Marketo - Documentazione prodotto
title: Abilita contenuto predittivo nelle e-mail
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Abilita contenuto predittivo nelle e-mail {#enable-predictive-content-in-emails}

Fai prevedere una o più immagini nel tuo messaggio e-mail, adattando l&#39;esperienza a ciascun destinatario.

>[!NOTE]
>
>Si consiglia di abilitare più di cinque elementi di contenuto per categoria e per origine (e-mail, rich media, barra) prima di testare e utilizzare Predictive Content. Più contenuto offre un risultato predittivo migliore.

>[!PREREQUISITES]
>
>Prima di abilitare Predictive Content. è necessario:
>
>* [Preparare il contenuto predittivo](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md)
>* [Approvare un titolo per il contenuto predittivo](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## Aggiunta di contenuti predittivi tramite l&#39;editor di e-mail 2.0 {#adding-predictive-content-using-the-email-editor}

1. Fate clic su **Attività marketing**.

   ![](assets/one.png)

1. Selezionate il messaggio e-mail e fate clic su **Modifica bozza**.

   ![](assets/two.png)

1. Fate clic sull’immagine da rendere predittiva. Quando viene visualizzata l&#39;icona a forma di ingranaggio, fate clic su di essa e selezionate **Abilita contenuto`AI`** (Content`AI` è il nome precedente per Contenuto predittivo).

   ![](assets/three.png)

1. Per selezionare una o più categorie, fare clic sul menu a discesa **Categorie**, effettuare le selezioni e fare clic su **Applica**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >La scelta di categorie specifiche o la modifica del layout predittivo è facoltativa.

1. L&#39;immagine è ora predittiva. Ripetete i passaggi 3 e 4 per ulteriori immagini (se necessario).

   ![](assets/five.png)

1. Per visualizzare l&#39;anteprima del messaggio e-mail, fate clic su **Anteprima** nell&#39;angolo superiore destro.

   ![](assets/six.png)

1. Per visualizzare diverse immagini possibili, fare clic su **Aggiorna**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >L&#39;immagine non viene selezionata **_finché il destinatario non apre l&#39;e-mail_**. Quello che vedete nell&#39;anteprima è solo un esempio, e non sarà necessariamente l&#39;immagine che il destinatario vede.

1. Dopo aver visualizzato l&#39;anteprima del messaggio e-mail, fare clic sul menu a discesa **Azioni anteprima** e selezionare **Approva e Chiudi**. Oppure, se è ancora necessario apportare modifiche, fare clic su **Modifica bozza** a destra.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Quando si invia un campione, viene selezionata un&#39;immagine casuale.

Dopo l&#39;approvazione, l&#39;e-mail sarà dotata di contenuti predittivi e pronta per l&#39;invio!

>[!CAUTION]
>
>Una volta che il destinatario apre il messaggio e-mail, le immagini predittive vengono bloccate. Se il contenuto viene rimosso in un secondo momento, i destinatari vedranno un&#39;immagine non corretta in cui si trova il contenuto.

## Aggiunta di contenuti predittivi quando non si utilizza l&#39;editor di e-mail 2.0 {#adding-predictive-content-when-not-using-the-email-editor}

Se non state utilizzando un modello [E-mail 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md), l&#39;aggiunta di contenuto predittivo al messaggio e-mail può essere fatta semplicemente assegnando un&#39;immagine nel modello come elemento immagine modificabile Marketo.

Informazioni sulla [sintassi specifica di Marketo](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements).

Di seguito è riportato un esempio di come dovrebbe essere il codice (questo è solo un esempio, non copiate esattamente il codice riportato di seguito).

**Esempio**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
