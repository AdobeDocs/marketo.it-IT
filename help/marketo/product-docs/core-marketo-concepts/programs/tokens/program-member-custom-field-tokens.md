---
unique-page-id: 1147114
description: Token di campo personalizzati per i membri del programma - Documentazione di Marketo - Documentazione del prodotto
title: Token campo personalizzato membro programma
exl-id: 3046dec8-b885-4b08-baa9-896bcf3594b2
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Token campo personalizzato membro programma {#program-member-custom-field-tokens}

## Supporto token per i campi personalizzati dei membri del programma {#token-support-for-program-member-custom-fields}

Sul pannello posteriore delle funzioni Campi personalizzati membro del programma, è in corso l&#39;estensione del supporto per i campi personalizzati membro del programma nei framework dei token.

I token PMCF saranno supportati nel dominio membro della famiglia di token.

I token dei membri vengono utilizzati per i campi che rientrano nell’ambito di Membro del programma. Allo stato attuale, i token membro vengono utilizzati anche per inserire valori univoci dai partner di servizi integrati. `{{member.webinar url}}` Il token risolve automaticamente l’URL univoco di conferma della persona generato dal provider di servizi. {{member.registration code}} viene risolto nel codice di registrazione fornito dal provider di servizi.

>[!NOTE]
>
>* I campi personalizzati dei membri del programma possono essere utilizzati solo nel contesto di un programma.
>* I token dei campi personalizzati dei membri del programma non possono essere utilizzati in: preheader e-mail, Token di data in Wait Steps o Snippet.
>* Lo stato dei membri del programma non è supportato nei token dei membri.

## Utilizzo dei token dei campi personalizzati dei membri del programma nelle risorse {#using-program-member-custom-field-tokens-in-assets}

Puoi inserire token dei campi personalizzati dei membri del programma in e-mail, pagine di destinazione, SMS, notifiche push e webhook.

**E-mail**

1. Seleziona l’e-mail desiderata e fai clic su **Modifica bozza**.

   ![](assets/program-member-custom-field-tokens-1.png)

1. Fai clic sull’icona Inserisci token.

   ![](assets/program-member-custom-field-tokens-2.png)

1. Trova e seleziona il token del campo personalizzato del membro del programma desiderato, immetti un valore predefinito e fai clic su **Inserisci**.

   ![](assets/program-member-custom-field-tokens-3.png)

1. Clic **Salva**.

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>Non dimenticare di approvare l’e-mail.

**Pagine di destinazione**

1. Seleziona la pagina di destinazione e fai clic su **Modifica bozza**.

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >Il designer della pagina di destinazione si apre in una nuova finestra.

1. Fare doppio clic sulla casella di testo RTF a cui si desidera aggiungere il token.

   ![](assets/program-member-custom-field-tokens-6.png)

1. Fai clic nel punto in cui desideri inserire il token, quindi fai clic sull’icona Inserisci token.

   ![](assets/program-member-custom-field-tokens-7.png)

1. Trova e seleziona il token desiderato.

   ![](assets/program-member-custom-field-tokens-8.png)

1. Inserisci un valore predefinito e fai clic su **Inserisci**.

   ![](assets/program-member-custom-field-tokens-9.png)

1. Clic **Salva**.

   ![](assets/program-member-custom-field-tokens-10.png)

**SMS**

1. Seleziona l’SMS desiderato e fai clic su **Modifica bozza**.

   ![](assets/program-member-custom-field-tokens-11.png)

1. Fai clic su **`{{ Token`** pulsante.

   ![](assets/program-member-custom-field-tokens-12.png)

1. Individua e seleziona il token del campo personalizzato del membro del programma desiderato. Immettere un valore predefinito e fare clic su Inserisci.

   ![](assets/program-member-custom-field-tokens-13.png)

1. Fai clic sul menu a discesa Azioni SMS e seleziona **Approva e chiudi**.

   ![](assets/program-member-custom-field-tokens-14.png)

**Notifiche push**

1. Seleziona la notifica push desiderata e fai clic su **Modifica bozza**.

   ![](assets/program-member-custom-field-tokens-15.png)

1. Clic **Notifica push**.

   ![](assets/program-member-custom-field-tokens-16.png)

1. Fai clic sul messaggio nell’editor e fai clic sul pulsante `{{` per ottenere il selettore del token.

   ![](assets/program-member-custom-field-tokens-17.png)

1. Individua e seleziona il token del campo personalizzato del membro del programma desiderato. Immetti un valore predefinito e fai clic su **Inserisci**.

   ![](assets/program-member-custom-field-tokens-18.png)

1. Clic **Fine** per salvare ed uscire (oppure **Successivo** per prima cosa).

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>Se il campo personalizzato Membro del programma per un membro del programma non contiene alcun valore, il token verrà sostituito con il valore predefinito, se fornito.

## Utilizzo dei token di campo personalizzati dei membri del programma nelle campagne {#using-program-member-custom-field-tokens-in-campaigns}

I token di campo personalizzati dei membri del programma possono essere utilizzati in:

* Crea attività
* Crea attività in Microsoft
* Momenti di interesse
* Azioni di flusso per cambiare il valore dei dati
* Webhook
