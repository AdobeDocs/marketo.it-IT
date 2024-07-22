---
unique-page-id: 2359422
description: Personalizzazione di un’e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Personalizzazione di un’e-mail
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Personalizzazione di un’e-mail {#personalize-an-email}

## Missione: rendi le e-mail personali aggiungendo token di dati {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configurazione e aggiunta di una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Inviare un messaggio di posta elettronica](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [Goccia, Goccia, Alimentazione](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## Passaggio 1: selezionare un messaggio e-mail da personalizzare {#step-select-an-email-to-personalize}

1. Seleziona una delle e-mail di sviluppo create nella [vittoria rapida precedente](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"} e fai clic su **[!UICONTROL Crea bozza]**.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >In questo modo viene creata una copia dell’e-mail come bozza. Ricordati di approvare la bozza per far sì che le modifiche vengano pubblicate.

Se non hai attivato un blocco popup, l’editor e-mail si aprirà in una nuova scheda/finestra. In caso contrario, fare clic due volte su **[!UICONTROL Crea bozza]**.

## Passaggio 2: rendi il venditore il mittente {#step-make-the-salesperson-the-sender}

1. Seleziona il campo **[!UICONTROL Da]**, evidenzia e **elimina** il nome corrente.

   ![](assets/personalize-an-email-2.png)

1. Fai clic sull&#39;icona **Token** a destra del campo **[!UICONTROL From]**.

   ![](assets/personalize-an-email-3.png)

1. Trova e seleziona il token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/personalize-an-email-4.png)

1. Digita il nome della tua società e un trattino per il **Valore predefinito** per assicurarti che venga visualizzato qualcosa nel caso in cui il nome del rappresentante di vendita non sia disponibile. Fare clic su **Inserisci**.

   ![](assets/personalize-an-email-5.png)

1. Premi la barra spaziatrice nel campo **[!UICONTROL From]**, assicurandoti che il cursore lampeggi in uno spazio dopo il token appena inserito. Quindi fai di nuovo clic sull&#39;icona **Token**.

   ![](assets/personalize-an-email-6.png)

1. Trova e seleziona il token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/personalize-an-email-7.png)

1. Digitare &quot;Vendite&quot; per il **Valore predefinito** e fare clic su **Inserisci**.

   ![](assets/personalize-an-email-8.png)

## Passaggio 3: aggiungi il nome del lead all’e-mail {#step-add-the-leads-name-to-the-email}

1. Seleziona la sezione modificabile superiore, fai clic sull&#39;icona ingranaggio e seleziona **[!UICONTROL Modifica]**.

   ![](assets/personalize-an-email-9.png)

1. Aggiungi uno spazio dopo &quot;Hello&quot; e posiziona il cursore davanti alla virgola, quindi fai clic sull&#39;icona **Inserisci token**.

   ![](assets/personalize-an-email-10.png)

1. Trova e seleziona il token **`{{lead.First Name}}`**.

   ![](assets/personalize-an-email-11.png)

1. Immetti &quot;Friend&quot; (o qualsiasi etichetta desiderata) nel campo **[!UICONTROL Valore predefinito]** e fai clic su **[!UICONTROL Inserisci]**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >Includi sempre un valore predefinito per i token; in questo modo il valore predefinito verrà visualizzato nell’e-mail se manca parte delle informazioni personali.

1. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/personalize-an-email-13.png)

1. In **[!UICONTROL Azioni e-mail]** e seleziona **[!UICONTROL Approva e chiudi]**.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>Vuoi un rapido aggiornamento su come inviarti l’e-mail? Consulta [Inviare un messaggio e-mail ](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}.

### Missione completata {#mission-complete}

Congratulazioni, hai personalizzato la tua e-mail!

<br> 

[Missione ◄ 6: gocciolamento, gocciolamento, crescita](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Missione 8: avvisare il rappresentante commerciale ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
