---
unique-page-id: 2359422
description: Personalizzazione di un'e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Personalizzare un’e-mail
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: ht
source-wordcount: '319'
ht-degree: 100%

---

# Personalizzare un’e-mail {#personalize-an-email}

## Missione: rendere le e-mail personali aggiungendo token di dati {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configurare e aggiungere una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Inviare più e-mail](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [Drip, Drip, Norture](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## Passaggio 1: selezionare un messaggio e-mail da personalizzare {#step-select-an-email-to-personalize}

1. Seleziona una delle e-mail di nurturing creata nella [nei risultati rapidi precedenti](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"} e fai clic su **[!UICONTROL Create draft]**.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >In questo modo viene creata una copia dell&#39;e-mail come bozza. Ricordati di approvare la bozza per far sì che le modifiche vengano pubblicate.

Se non hai attivato un blocco pop-up, l&#39;editor e-mail si aprirà in una nuova scheda/finestra. In caso contrario, fai clic due volte su **[!UICONTROL Create Draft]**.

## Passaggio 2: rendere il venditore il mittente {#step-make-the-salesperson-the-sender}

1. Seleziona il campo **[!UICONTROL From]**, evidenzia e **elimina** il nome corrente.

   ![](assets/personalize-an-email-2.png)

1. Fai clic sull&#39;icona **Token** a destra del campo **[!UICONTROL From]**.

   ![](assets/personalize-an-email-3.png)

1. Trova e seleziona il token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/personalize-an-email-4.png)

1. Digita il nome della tua azienda e un trattino per il **Valore predefinito** per garantire che venga visualizzato qualcosa nel caso in cui il nome del rappresentante di vendita non sia disponibile. Fai clic su **Inserisci**.

   ![](assets/personalize-an-email-5.png)

1. Premi la barra spaziatrice nel campo **[!UICONTROL From]**, assicurandoti che il cursore lampeggi uno spazio dopo il token appena inserito. Quindi fai di nuovo clic sull&#39;icona **Token**.

   ![](assets/personalize-an-email-6.png)

1. Trova e seleziona il token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/personalize-an-email-7.png)

1. Digita &quot;Vendite&quot; per il **Valore predefinito** e fai clic su **Inserisci**.

   ![](assets/personalize-an-email-8.png)

## Passaggio 3: aggiungere il nome del lead all&#39;e-mail {#step-add-the-leads-name-to-the-email}

1. Seleziona la sezione modificabile superiore, fai clic sull&#39;icona ingranaggio e seleziona **[!UICONTROL Edit]**.

   ![](assets/personalize-an-email-9.png)

1. Aggiungi uno spazio dopo &quot;Hello&quot; e posiziona il cursore davanti alla virgola, quindi fai clic sull&#39;icona **Inserisci token**.

   ![](assets/personalize-an-email-10.png)

1. Trova e seleziona il token **`{{lead.First Name}}`**.

   ![](assets/personalize-an-email-11.png)

1. Immetti &quot;Amico&quot; (o qualsiasi etichetta desiderata) nel campo **[!UICONTROL Default Value]** e fai clic su **[!UICONTROL Insert]**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >Includi sempre un valore predefinito per i token; in questo modo il valore predefinito verrà visualizzato nell&#39;e-mail se manca parte delle informazioni personali.

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/personalize-an-email-13.png)

1. In **[!UICONTROL Email Actions]**, seleziona **[!UICONTROL Approve and Close]**.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>Vuoi un rapido aggiornamento su come inviarti l&#39;e-mail? Consulta [Inviare più e-mail ](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}.

### Missione completata {#mission-complete}

Congratulazioni, hai personalizzato la tua e-mail!

<br> 

[◄ Missione 6: Drip, Drip, Nurture](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Missione 8: avvisare il rsponsabile delle vendite ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
