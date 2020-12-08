---
unique-page-id: 2359422
description: Personalizzare un'e-mail - Documenti Marketo - Documentazione prodotto
title: Personalizzare un'e-mail
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---


# Personalizzare un&#39;e-mail {#personalize-an-email}

## Missione: Rendere le e-mail personali aggiungendo token di dati {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

>[!NOTE]
>
>**Prerequisiti**
>
>* [Configurazione e aggiunta di una persona](get-set-up-and-add-a-person.md)
>* [Invio di un messaggio e-mail con esplosione](send-an-email.md)
>* [Drip, Drip, Cura](drip-drip-nurture.md)


## Passaggio 1: Selezionare un&#39;e-mail da personalizzare {#step-select-an-email-to-personalize}

1. Selezionate una delle e-mail di nutrizione create nella vittoria [rapida](drip-drip-nurture.md) precedente e fate clic su **Modifica bozza**.

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >Viene creata una copia dell’e-mail come bozza. È necessario approvare la bozza affinché le modifiche diventino attive.

   **Modifica bozza**

Se non avete attivato il blocco dei pop-up, l&#39;editor e-mail si aprirà in una nuova scheda o finestra. In caso contrario, fate clic due volte.

## Passaggio 2: Imposta il venditore come mittente {#step-make-the-salesperson-the-sender}

1. Selezionare il campo **Da** , evidenziare ed **eliminare** il nome corrente.

   ![](assets/two-5.png)

1. Fate clic sull&#39;icona **Token** a destra del campo **Da** .

   ![](assets/three-4.png)

1. Trova e seleziona il **`{{lead.Lead Owner First Name}}`** token.

   ![](assets/four-3.png)

1. Digitare il nome della società e un trattino per il valore **** predefinito per assicurarsi che venga visualizzato qualcosa nel caso in cui il nome del rappresentante della vendita non sia disponibile. Fate clic su **Inserisci**.

   ![](assets/five-4.png)

1. Premete la barra spaziatrice nel campo **Da** , assicurandovi che il cursore lampeggi uno spazio dopo il token appena inserito. Quindi fate di nuovo clic sull&#39;icona **Token** .

   ![](assets/six-4.png)

1. Trova e seleziona il **`{{lead.Lead Owner Last Name}}`** token.

   ![](assets/seven-5.png)

1. Digitare &quot;Vendite&quot; per il valore **** predefinito e fare clic su **Inserisci**.

   ![](assets/eight-3.png)

## Passaggio 3: Aggiungi il nome del lead all’e-mail {#step-add-the-leads-name-to-the-email}

1. Selezionate la sezione modificabile superiore, fate clic sull&#39;icona a forma di ingranaggio e selezionate **Modifica**.

   ![](assets/nine-2.png)

1. Aggiungi uno spazio dopo &quot;Hello&quot; e posiziona il cursore davanti alla virgola, quindi fai clic sull&#39;icona **Inserisci token** .

   ![](assets/ten-4.png)

1. Trova e seleziona il **`{{lead.First Name}}`** token.

   ![](assets/eleven-4.png)

1. Immettere &quot;Friend&quot; (o qualsiasi etichetta desiderata) nel campo Valore **** predefinito e fare clic su **Inserisci**.

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >Includi sempre un valore predefinito per i token; in questo modo il valore predefinito verrà visualizzato nel messaggio e-mail se manca parte delle informazioni personali.

1. Fate clic su **Salva**.

   ![](assets/thirteen-3.png)

1. Chiudete la scheda o la finestra dell’editor e-mail.

   ![](assets/fourteen-3.png)

1. In Azioni **e-** mail, selezionare **Approva bozza**.

   ![](assets/fifteen-3.png)

>[!TIP]
>
>Hai bisogno di un aggiornamento rapido su come inviarti l&#39;e-mail? Consultate [Inviare un messaggio e-mail](send-an-email.md)con esplosione.

### Video {#watch-a-video}

`<iframe width="630" height="470" src="//play.vidyard.com/iRnqxMyJg6VKyuPeuxmHFb.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`

### Missione completata {#mission-complete}

Congratulazioni, hai personalizzato la tua email!

<br> 

[◄ Missione 6: Drip, Drip, Nurture](drip-drip-nurture.md) [Mission 8: Avvisa il rappresentante commerciale ►](alert-the-sales-rep.md)