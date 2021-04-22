---
unique-page-id: 2359422
description: Personalizzare un’e-mail - Documenti Marketo - Documentazione del prodotto
title: Personalizzare un’e-mail
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Personalizzare un&#39;e-mail {#personalize-an-email}

## Missione: Rendi le tue e-mail personali aggiungendo token di dati {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configurazione e aggiunta di una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)
>* [Invia un&#39;e-mail di avviso](/help/marketo/getting-started/quick-wins/send-an-email.md)
>* [Asciugatura, Asciugatura, Alimentazione](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)


## Passaggio 1: Selezionare un&#39;e-mail da personalizzare {#step-select-an-email-to-personalize}

1. Seleziona una delle e-mail di nutrizione create nella [precedente vittoria rapida](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md) e fai clic su **Modifica bozza**.

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >Viene creata una copia dell’e-mail come bozza. È necessario approvare la bozza affinché le modifiche diventino attive.

Se non hai attivato un blocco dei popup, l’editor e-mail si aprirà in una nuova scheda/finestra. In caso contrario, fare due volte clic su **Modifica bozza**.

## Passaggio 2: Rendi il venditore il mittente {#step-make-the-salesperson-the-sender}

1. Selezionare il campo **Da**, evidenziare e **eliminare** il nome corrente.

   ![](assets/two-5.png)

1. Fai clic sull&#39;icona **Token** a destra del campo **Da** .

   ![](assets/three-4.png)

1. Trova e seleziona il token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/four-3.png)

1. Digita il nome della tua azienda e un trattino per **Valore predefinito** per assicurarti che venga visualizzato qualcosa nel caso in cui il nome del rappresentante di vendita non sia disponibile. Fare clic su **Inserisci**.

   ![](assets/five-4.png)

1. Premi la barra spaziatrice nel campo **Da** , assicurandoti che il cursore lampeggi uno spazio dopo il token appena inserito. Quindi fai di nuovo clic sull&#39;icona **Token** .

   ![](assets/six-4.png)

1. Trova e seleziona il token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/seven-5.png)

1. Digita &quot;Sales&quot; per il **Valore predefinito** e fai clic su **Inserisci**.

   ![](assets/eight-3.png)

## Passaggio 3: Aggiungi il nome del lead all’e-mail {#step-add-the-leads-name-to-the-email}

1. Seleziona la sezione superiore modificabile, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Modifica**.

   ![](assets/nine-2.png)

1. Aggiungi uno spazio dopo &quot;Ciao&quot; e posiziona il cursore davanti alla virgola, quindi fai clic sull&#39;icona **Inserisci token**.

   ![](assets/ten-4.png)

1. Trova e seleziona il token **`{{lead.First Name}}`**.

   ![](assets/eleven-4.png)

1. Inserisci &quot;Amico&quot; (o qualsiasi etichetta desiderata) nel campo **Valore predefinito** e fai clic su **Inserisci**.

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >Includi sempre un valore predefinito per i token; in questo modo, il valore predefinito verrà visualizzato nell’e-mail se manca parte delle informazioni personali.

1. Fare clic su **Salva**.

   ![](assets/thirteen-3.png)

1. Chiudi la scheda/finestra dell’editor e-mail.

   ![](assets/fourteen-3.png)

1. In **Azioni e-mail**, seleziona **Approva bozza**.

   ![](assets/fifteen-3.png)

>[!TIP]
>
>Ti serve un aggiornamento rapido su come inviarti l’e-mail? Consulta [Inviare un messaggio e-mail](/help/marketo/getting-started/quick-wins/send-an-email.md).

### Missione completata {#mission-complete}

Congratulazioni, hai personalizzato la tua e-mail!

<br> 

[◄ Missione 6: Asciugatura, Asciugatura, Alimentazione](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Missione 8 Avvisare il rappresentante commerciale ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
