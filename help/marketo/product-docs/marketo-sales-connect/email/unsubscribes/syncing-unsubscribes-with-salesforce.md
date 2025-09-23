---
unique-page-id: 14746188
description: Sincronizzazione degli annullamenti dell’abbonamento con Salesforce - Documentazione di Marketo - Documentazione del prodotto
title: Sincronizzazione degli annullamenti delle iscrizioni con Salesforce
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 2%

---

# Sincronizzazione degli annullamenti iscrizione con [!DNL Salesforce] {#syncing-unsubscribes-with-salesforce}

## Requisiti per l&#39;annullamento dell&#39;abbonamento alla sincronizzazione con [!DNL Salesforce] {#requirements-for-unsubscribes-to-sync-to-salesforce}

* La sincronizzazione degli annullamenti dell’abbonamento deve essere abilitata (per la sincronizzazione notturna)
* Il campo Opt Out deve essere installato in [!DNL Salesforce]
* I record della persona in [!DNL Sales Connect] devono avere un ID [!DNL Salesforce]

**Annullamenti iscrizione push**

Quando si raccoglie un annullamento dell&#39;iscrizione in [!DNL Sales Connect], questo viene inviato a [!DNL Salesforce] in tempo reale e viene aggiornato uno dei campi di rinuncia selezionati per la sincronizzazione. Se hai disattivato la sincronizzazione di [!DNL Salesforce], l&#39;annullamento dell&#39;iscrizione verrà comunque inviato al servizio di rinuncia all&#39;e-mail.

**Sincronizzazione annullamento abbonamento**

Dopo aver attivato la sincronizzazione per l’annullamento dell’abbonamento (passaggio 3 di seguito), verrà attivata la sincronizzazione notturna. La sincronizzazione viene eseguita una volta al giorno intorno alle 20.00 PST. :00 Sincronizzerà in modo bidirezionale tutti gli annullamenti di abbonamenti in Marketo Sales con il campo Opt Out in Salesforce.

## Configura sincronizzazione annullamento sottoscrizioni a [!DNL Salesforce] {#configure-unsubscribe-sync-to-salesforce}

Gli utenti possono decidere se sincronizzare gli annullamenti degli abbonamenti con il campo standard Email Opt Out (Rinuncia e-mail) con cui può sincronizzarsi Marketo, oppure con il campo Marketo Sales Opt Out (Rinuncia alle vendite) in modo da poter distinguere gli annullamenti degli abbonamenti alle vendite e agli marketing.

1. Vai all&#39;[applicazione Web](https://toutapp.com/login), fai clic sull&#39;icona a forma di ingranaggio e seleziona **[!UICONTROL Settings]**.

   ![](assets/one-1.png)

1. In [!UICONTROL Admin Settings] selezionare **[!UICONTROL Unsubscribes]**.

   ![](assets/two-2.png)

1. Fare clic su **[!UICONTROL Syncing to Salesforce]**, quindi attivare la sincronizzazione notturna.

   ![](assets/three-2.png)

1. Seleziona il campo a cui desideri sincronizzare.

   ![](assets/4.png)

   | Campo | Descrizione |
   |---|---|
   | **[!UICONTROL Sync to Salesforce Opt Out field]** | Selezionata per impostazione predefinita, aggiorna solo il campo di rinuncia [!DNL Salesforce]. |
   | **[!UICONTROL Sync to Marketo Sales Opt Out field]** | Se si desidera separare gli annullamenti degli abbonamenti alle vendite e al marketing, scegliere questa opzione per aggiornare il campo aggiuntivo [Marketo Sales Opt Out.](#msoo) |

## Installazione del campo Rinuncia nel layout di pagina {#installing-the-opt-out-field-in-the-page-layout}

**Rinuncia e-mail**

Rinuncia e-mail è un campo standard in [!DNL Salesforce] disponibile per l&#39;installazione da [!DNL Salesforce]. È necessario essere un amministratore [!DNL Salesforce] per installarlo.

1. Vai a [Salesforce.com](https://salesforce.com) e accedi.

   ![](assets/five-1.png)

1. Fare clic sul proprio nome utente e selezionare **[!UICONTROL Setup]**.

   ![](assets/six-1.png)

1. Nella casella di ricerca rapida cercare Contatto o Lead. In questo caso, il campo verrà installato nel layout della pagina Contatto, ma sarà necessario eseguire l&#39;installazione per entrambi i record persona.

   ![](assets/seven-1.png)

1. Seleziona **[!UICONTROL Page Layouts]**.

   ![](assets/eight-1.png)

1. Selezionare **[!UICONTROL Edit]** accanto al layout di pagina a cui si desidera aggiungere il campo.

   ![](assets/nine.png)

1. Seleziona **[!UICONTROL Fields]**.

   ![](assets/ten.png)

1. Trascina [!UICONTROL Email Opt Out] nel layout della pagina.

   ![](assets/11.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/twelve.png)

## Rinuncia alle vendite Marketo {#marketo-sales-opt-out}

Il campo Marketo Sales Opt Out è un campo personalizzato disponibile per gli utenti che hanno installato le personalizzazioni di Marketo [!DNL Sales Connect].

Dopo aver installato correttamente le personalizzazioni di Marketo [!DNL Sales Connect] in [!DNL Salesforce], verrà visualizzato il campo di rinuncia alle vendite di Marketo disponibile.
