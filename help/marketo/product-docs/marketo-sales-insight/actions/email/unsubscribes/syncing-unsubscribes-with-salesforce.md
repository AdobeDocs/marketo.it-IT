---
description: Sincronizzazione degli annullamenti dell’abbonamento con Salesforce - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione degli annullamenti di abbonamenti con Salesforce
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
source-git-commit: ec79f405f975f2179aae94ec5556808785d7c594
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Sincronizzazione degli annullamenti di abbonamenti con Salesforce {#syncing-unsubscribes-with-salesforce}

Se desideri sincronizzare gli annullamenti dell’abbonamento con un campo di rinuncia in Salesforce, puoi utilizzare la sincronizzazione degli annullamenti dell’abbonamento di Salesforce.

## Requisiti per annullare l’abbonamento a Sync to Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* La sincronizzazione degli annullamenti dell’abbonamento deve essere abilitata (per la sincronizzazione notturna)
* Il campo Opt Out deve essere installato in Salesforce
* I record persona in Marketo Sales devono avere un ID Salesforce

**Annullamenti iscrizione push**

Quando un utente riceve un annullamento dell’abbonamento in Marketo Sales, lo inviamo a Salesforce in tempo reale e aggiorna uno dei campi di rinuncia selezionati per la sincronizzazione con. Se hai disattivato la sincronizzazione con Salesforce, invieremo comunque l’annullamento dell’iscrizione alla rinuncia all’e-mail.

**Sincronizzazione per annullamento iscrizione**

Dopo aver attivato la sincronizzazione per l’annullamento dell’iscrizione (passaggio 3 di seguito), la sincronizzazione notturna verrà attivata. La sincronizzazione viene eseguita una volta al giorno intorno alle 20:00 PST. Sincronizzerà bidirezionalmente tutti gli annullamenti di abbonamenti in Marketo Sales con il campo Opt Out in Salesforce.

>[!NOTE]
>
>La sincronizzazione dell’annullamento degli abbonamenti con Salesforce sincronizzerà gli annullamenti degli abbonamenti, ma non sincronizzerà i nuovi abbonamenti. Se desideri rimuovere un abbonamento a Marketo Sales e Salesforce, deseleziona l’opzione per annullare l’abbonamento in Salesforce e rimuovi l’annullamento dell’abbonamento in Marketo Sales.

## Configurare la sincronizzazione degli annullamenti dell’abbonamento con Salesforce {#configure-unsubscribe-sync-to-salesforce}

Gli utenti possono decidere se sincronizzare gli annullamenti degli abbonamenti con il campo standard Email Opt Out (Rinuncia e-mail) con cui può sincronizzarsi Marketo, oppure con il campo Marketo Sales Opt Out (Rinuncia alle vendite) in modo da poter distinguere gli annullamenti degli abbonamenti alle vendite e agli marketing.

1. Fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. In Impostazioni amministratore seleziona **Annulla iscrizione**.

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. Fai clic su **Integrazioni** scheda. In Sincronizza con Salesforce, abilita la sincronizzazione notturna.

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. Seleziona il campo a cui desideri sincronizzare.

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | Campo | Descrizione |
   |---|---|
   | **Sincronizza con il campo di rinuncia Salesforce** | Selezionata per impostazione predefinita, aggiorna solo il campo Rinuncia Salesforce. |
   | **Sincronizza con il campo Marketo Sales Opt Out** | Se si desidera separare gli annullamenti degli abbonamenti alle vendite e al marketing, scegliere questa opzione per aggiornare ulteriori [Campo Rinuncia vendite Marketo.](#msoo) |

## Installazione del campo Rinuncia nel layout di pagina {#installing-the-opt-out-field-in-the-page-layout}

**Rinuncia e-mail**

Rinuncia e-mail è un campo standard in Salesforce disponibile per l’installazione da Salesforce. Per installarlo, devi essere un amministratore Salesforce.

1. Vai a [Salesforce.com](https://salesforce.com) e accedi.

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. Fai clic sul nome utente e seleziona **Configurazione**.

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. Nella casella di ricerca rapida cercare Contatto o Lead. In questo caso, il campo verrà installato nel layout della pagina Contatto, ma sarà necessario eseguire l&#39;installazione per entrambi i record persona.

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. Seleziona **Layout di pagina**.

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. Seleziona **Modifica** accanto al layout di pagina a cui si desidera aggiungere il campo.

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. Seleziona **Campi**.

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. Trascina e rilascia la rinuncia e-mail nel layout della pagina.

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. Clic **Salva**.

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Rinuncia alle vendite Marketo {#marketo-sales-opt-out}

Il campo Rinuncia vendite Marketo è un campo personalizzato disponibile per gli utenti che hanno installato il pacchetto Marketo Sales Insight [dall’AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

Dopo aver installato correttamente il pacchetto Marketo Sales Insight dall’AppExchange in Salesforce, visualizzerai il campo Marketo Sales Opt Out disponibile.
