---
unique-page-id: 1147114
description: Token di campo personalizzati per i membri del programma - Documentazione di Marketo - Documentazione del prodotto
title: Token campo personalizzato del membro del programma
exl-id: 3046dec8-b885-4b08-baa9-896bcf3594b2
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 5%

---

# Token campo personalizzato del membro del programma {#program-member-custom-field-tokens}

## Supporto token per i campi personalizzati dei membri del programma {#token-support-for-program-member-custom-fields}

Sul pannello posteriore delle funzioni Campi personalizzati membro del programma, è in corso l&#39;estensione del supporto per i campi personalizzati membro del programma nei framework dei token.

I token PMCF saranno supportati nel dominio membro della famiglia di token.

I token dei membri vengono utilizzati per i campi che rientrano nell’ambito di Membro del programma. Allo stato attuale, i token membro vengono utilizzati anche per inserire valori univoci dai partner di servizi integrati. Il token `{{member.webinar url}}` risolve automaticamente l&#39;URL di conferma univoco della persona generato dal provider di servizi. {{member.registration code}} viene risolto nel codice di registrazione fornito dal provider di servizi.

>[!NOTE]
>
>* I campi personalizzati dei membri del programma possono essere utilizzati solo nel contesto di un programma.
>* I token dei campi personalizzati dei membri del programma non possono essere utilizzati in: preheader e-mail, Token di data in Wait Steps o Snippet.
>* Lo stato dei membri del programma non è supportato nei token dei membri.

## Utilizzo dei token dei campi personalizzati dei membri del programma in Assets {#using-program-member-custom-field-tokens-in-assets}

Puoi inserire token dei campi personalizzati dei membri del programma in e-mail, pagine di destinazione, SMS, notifiche push e webhook.

**E-Mail**

1. Selezionare l&#39;e-mail desiderata e fare clic su **[!UICONTROL Edit Draft]**.

   ![](assets/program-member-custom-field-tokens-1.png)

1. Fai clic sull’icona Inserisci token.

   ![](assets/program-member-custom-field-tokens-2.png)

1. Individuare e selezionare il token del campo personalizzato del membro del programma desiderato, immettere un valore predefinito e fare clic su **[!UICONTROL Insert]**.

   ![](assets/program-member-custom-field-tokens-3.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>Non dimenticare di approvare l’e-mail.

**Pagine di destinazione**

1. Selezionare la pagina di destinazione e fare clic su **[!UICONTROL Edit Draft]**.

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

1. Immettere un valore predefinito e fare clic su **[!UICONTROL Insert]**.

   ![](assets/program-member-custom-field-tokens-9.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/program-member-custom-field-tokens-10.png)

**SMS**

1. Selezionare l&#39;SMS desiderato e fare clic su **[!UICONTROL Edit Draft]**.

   ![](assets/program-member-custom-field-tokens-11.png)

1. Fare clic sul pulsante **`{{ Token`**.

   ![](assets/program-member-custom-field-tokens-12.png)

1. Individua e seleziona il token del campo personalizzato del membro del programma desiderato. Immettere [!UICONTROL default value] e fare clic su **[!UICONTROL Insert]**.

   ![](assets/program-member-custom-field-tokens-13.png)

1. Fare clic sul menu a discesa Azioni SMS e selezionare **[!UICONTROL Approve & Close]**.

   ![](assets/program-member-custom-field-tokens-14.png)

**Notifiche push**

1. Selezionare la notifica push desiderata e fare clic su **[!UICONTROL Edit Draft]**.

   ![](assets/program-member-custom-field-tokens-15.png)

1. Fai clic su **[!UICONTROL Push Notification]**.

   ![](assets/program-member-custom-field-tokens-16.png)

1. Fai clic sul messaggio nell&#39;editor e fai clic sul pulsante `{{` per ottenere il selettore del token.

   ![](assets/program-member-custom-field-tokens-17.png)

1. Individua e seleziona il token del campo personalizzato del membro del programma desiderato. Immettere un valore predefinito e fare clic su **[!UICONTROL Insert]**.

   ![](assets/program-member-custom-field-tokens-18.png)

1. Fare clic su **[!UICONTROL Finish]** per salvare e uscire (oppure su **[!UICONTROL Next]** per rivedere prima).

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>Se il campo personalizzato Membro del programma per un membro del programma non contiene alcun valore, il token verrà sostituito con il valore predefinito, se fornito.

## Utilizzo dei token di campo personalizzati dei membri del programma nelle campagne {#using-program-member-custom-field-tokens-in-campaigns}

I token di campo personalizzati dei membri del programma possono essere utilizzati in:

* Creare attività
* Creare attività in Microsoft
* Momenti di interesse
* Azioni di flusso per cambiare il valore dei dati
* Webhook
