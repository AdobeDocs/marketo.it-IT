---
unique-page-id: 2359422
description: Personalizzare un’e-mail - Documenti Marketo - Documentazione del prodotto
title: Personalizzare un’e-mail
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Personalizzare un’e-mail {#personalize-an-email}

## Missione: Rendere le e-mail personali aggiungendo token dati {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configurazione e aggiunta di una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [Invia un&#39;e-mail di avviso](/help/marketo/getting-started/quick-wins/send-an-email.md){target=&quot;_blank&quot;}
>* [Asciugatura, Asciugatura, Alimentazione](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target=&quot;_blank&quot;}


## Passaggio 1: Selezionare un’e-mail da personalizzare {#step-select-an-email-to-personalize}

1. Seleziona una delle e-mail di nutrizione create nel [vittoria rapida precedente](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target=&quot;_blank&quot;} e fai clic su **Modifica bozza**.

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >Viene creata una copia dell’e-mail come bozza. È necessario approvare la bozza affinché le modifiche diventino attive.

Se non hai attivato un blocco dei popup, l’editor e-mail si aprirà in una nuova scheda/finestra. In caso contrario, fai clic su **Modifica bozza** due volte.

## Passaggio 2: Rendi il venditore il mittente {#step-make-the-salesperson-the-sender}

1. Seleziona la **Da** campo, evidenziazione e **delete** il nome corrente.

   ![](assets/two-5.png)

1. Fai clic sul pulsante **Token** a destra della **Da** campo .

   ![](assets/three-4.png)

1. Trova e seleziona la **`{{lead.Lead Owner First Name}}`** token.

   ![](assets/four-3.png)

1. Digita il nome della tua azienda e un trattino per **Valore predefinito** per assicurarsi che venga visualizzato qualcosa nel caso in cui il nome del rappresentante di vendita non sia disponibile. Fai clic su **Inserisci**.

   ![](assets/five-4.png)

1. Premi la barra spaziatrice nel **Da** verificare che il cursore lampeggi uno spazio dopo il token appena inserito. Quindi fai clic sul pulsante **Token** icona di nuovo.

   ![](assets/six-4.png)

1. Trova e seleziona la **`{{lead.Lead Owner Last Name}}`** token.

   ![](assets/seven-5.png)

1. Digitare &quot;Vendite&quot; per **Valore predefinito** e fai clic su **Inserisci**.

   ![](assets/eight-3.png)

## Passaggio 3: Aggiungi il nome del lead all’e-mail {#step-add-the-leads-name-to-the-email}

1. Seleziona la sezione superiore modificabile, fai clic sull’icona a forma di ingranaggio e seleziona **Modifica**.

   ![](assets/nine-2.png)

1. Aggiungi uno spazio dopo &quot;Ciao&quot; e posiziona il cursore davanti alla virgola, quindi fai clic sul **Inserisci token** icona.

   ![](assets/ten-4.png)

1. Trova e seleziona la **`{{lead.First Name}}`** token.

   ![](assets/eleven-4.png)

1. Inserisci &quot;Amico&quot; (o qualsiasi etichetta che desideri) nel **Valore predefinito** campo e fai clic su **Inserisci**.

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >Includi sempre un valore predefinito per i token; in questo modo, il valore predefinito verrà visualizzato nell’e-mail se manca parte delle informazioni personali.

1. Fai clic su **Salva**.

   ![](assets/thirteen-3.png)

1. Chiudi la scheda/finestra dell’editor e-mail.

   ![](assets/fourteen-3.png)

1. Sotto **Azioni e-mail**, seleziona **Approva bozza**.

   ![](assets/fifteen-3.png)

>[!TIP]
>
>Ti serve un aggiornamento rapido su come inviarti l’e-mail? Vedi [Invia un&#39;e-mail di avviso](/help/marketo/getting-started/quick-wins/send-an-email.md){target=&quot;_blank&quot;}.

### Missione completata {#mission-complete}

Congratulazioni, hai personalizzato la tua e-mail!

<br> 

[◄ Missione 6: Asciugatura, Asciugatura, Alimentazione](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Missione 8 Avvisare il rappresentante commerciale ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
