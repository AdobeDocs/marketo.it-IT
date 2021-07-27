---
unique-page-id: 1147114
description: Token di campo personalizzati per i membri del programma - Documenti Marketo - Documentazione del prodotto
title: Token dei campi personalizzati dei membri del programma
exl-id: 3046dec8-b885-4b08-baa9-896bcf3594b2
source-git-commit: 30f56d93dfd5a600ef3ea75d352ede12c6104940
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Token dei campi personalizzati dei membri del programma {#program-member-custom-field-tokens}

## Supporto token per i campi personalizzati dei membri del programma {#token-support-for-program-member-custom-fields}

Sul retro delle funzionalità Campi personalizzati dei membri del programma, è in corso l’estensione del supporto per i campi personalizzati dei membri del programma nei framework dei token.

I token PMCF saranno supportati nel dominio membro della famiglia di token.

I token membri sono utilizzati per i campi che rientrano nell’ambito di partecipazione al programma. Allo stato attuale, i token degli Stati membri sono utilizzati anche per inserire valori univoci da partner di servizi integrati. `{{member.webinar url}}` il token risolve automaticamente l’URL di conferma univoco della persona generato dal provider di servizi. {{membro.registration code}} risolve il codice di registrazione fornito dal provider di servizi.

>[!NOTE]
>
>* I campi personalizzati dei membri del programma possono essere utilizzati solo nel contesto di un programma.
>* I token dei campi personalizzati dei membri del programma non possono essere utilizzati in: preintestazione e-mail, token di data in passaggi di attesa o snippet.
>* Lo stato dei membri del programma non è supportato nei token membri.


## Utilizzo dei token di campo personalizzati dei membri del programma nelle risorse {#using-program-member-custom-field-tokens-in-assets}

Puoi inserire token di campi personalizzati dei membri del programma in e-mail, pagine di destinazione, SMS, notifiche push e webhook.

**E-mail**

1. Seleziona l’e-mail desiderata e fai clic su **Modifica bozza**.

   ![](assets/program-member-custom-field-tokens-1.png)

1. Fai clic sull’icona Inserisci token .

   ![](assets/program-member-custom-field-tokens-2.png)

1. Trova e seleziona il Token di campo personalizzato del membro del programma desiderato, inserisci un valore predefinito e fai clic su **Inserisci**.

   ![](assets/program-member-custom-field-tokens-3.png)

1. Fare clic su **Salva**.

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>Non dimenticarti di approvare la tua e-mail.

**Pagine di destinazione**

1. Seleziona la pagina di destinazione e fai clic su **Modifica bozza**.

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >La finestra di progettazione della pagina di destinazione viene aperta in una nuova finestra.

1. Fare doppio clic sulla casella RTF a cui si desidera aggiungere il token.

   ![](assets/program-member-custom-field-tokens-6.png)

1. Fai clic nel punto in cui desideri che sia il token, quindi fai clic sull’icona Inserisci token .

   ![](assets/program-member-custom-field-tokens-7.png)

1. Trova e seleziona il token desiderato.

   ![](assets/program-member-custom-field-tokens-8.png)

1. Immetti un valore predefinito e fai clic su **Inserisci**.

   ![](assets/program-member-custom-field-tokens-9.png)

1. Fare clic su **Salva**.

   ![](assets/program-member-custom-field-tokens-10.png)

**SMS**

1. Seleziona l’SMS desiderato e fai clic su **Modifica bozza**.

   ![](assets/program-member-custom-field-tokens-11.png)

1. Fai clic sul pulsante **`{{ Token`** .

   ![](assets/program-member-custom-field-tokens-12.png)

1. Trova e seleziona il token campo personalizzato del membro del programma desiderato. Immettere un valore predefinito e fare clic su Inserisci.

   ![](assets/program-member-custom-field-tokens-13.png)

1. Fai clic sull’elenco a discesa Azioni SMS e seleziona **Approva e chiudi**.

   ![](assets/program-member-custom-field-tokens-14.png)

**Notifiche push**

1. Seleziona la notifica push desiderata e fai clic su **Modifica bozza**.

   ![](assets/program-member-custom-field-tokens-15.png)

1. Fai clic su **Notifica push**.

   ![](assets/program-member-custom-field-tokens-16.png)

1. Fai clic sul messaggio nell’editor e fai clic sul pulsante `{{` per ottenere il selettore dei token.

   ![](assets/program-member-custom-field-tokens-17.png)

1. Trova e seleziona il token campo personalizzato del membro del programma desiderato. Immetti un valore predefinito e fai clic su **Inserisci**.

   ![](assets/program-member-custom-field-tokens-18.png)

1. Fare clic su **Fine** per salvare e uscire (oppure su **Avanti** per eseguire prima la revisione).

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>Se il campo personalizzato del membro del programma per un membro del programma non ha valore, il token verrà sostituito con il valore predefinito, se specificato.

## Utilizzo dei token di campo personalizzati dei membri del programma nelle campagne {#using-program-member-custom-field-tokens-in-campaigns}

I token di campo personalizzati dei membri del programma possono essere utilizzati in:

* Crea attività
* Crea attività in Microsoft
* Momenti interessanti
* Modificare le azioni del flusso di dati
* Webhook
