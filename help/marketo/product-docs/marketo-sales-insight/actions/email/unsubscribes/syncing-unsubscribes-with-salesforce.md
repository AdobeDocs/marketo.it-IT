---
description: Sincronizzazione degli abbonamenti con Salesforce - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione degli abbonamenti con Salesforce
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
source-git-commit: 27ca6c3efc5d49729ca4473853688be9cc8cdbc9
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Sincronizzazione degli abbonamenti con Salesforce {#syncing-unsubscribes-with-salesforce}

## Requisiti per l&#39;annullamento della sottoscrizione alla sincronizzazione con Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* Annulla sincronizzazione deve essere abilitato (per la sincronizzazione notturna)
* Il campo Opt Out deve essere installato in Salesforce
* I record personali nelle vendite Marketo devono avere un ID Salesforce

**Annulla sottoscrizione push**

Quando viene raccolto un annullamento dell’abbonamento in Marketo Sales, lo inviamo in tempo reale a Salesforce e aggiorniamo uno dei campi Opt Out con cui hai selezionato la sincronizzazione. Se hai disabilitato la sincronizzazione di Salesforce, l’annullamento della sottoscrizione verrà comunque inviato alla rinuncia all’e-mail.

**Annulla sincronizzazione**

Dopo aver attivato la sincronizzazione dell’annullamento dell’abbonamento (passaggio 3 qui sotto) verrà attivata la sincronizzazione notturna. La sincronizzazione avviene una volta al giorno intorno alle 20:00 PST. Sincronizza bidirezionale tutti gli annullamenti di abbonamenti nelle vendite di Marketo con il campo Opt Out in Salesforce.

## Configurare Annulla sottoscrizione sincronizzazione con Salesforce {#configure-unsubscribe-sync-to-salesforce}

Gli utenti possono decidere se sincronizzare i propri annullamenti di abbonamenti con il campo Rifiuto e-mail standard con cui Marketo può anche eseguire la sincronizzazione, oppure possono sincronizzarsi con il campo Rinuncia alle vendite Marketo in modo che gli annullamenti di abbonamenti alle vendite e gli annullamenti di Marketing possano essere differenziati.

1. Fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. In Impostazioni amministratore, seleziona **Annulla sottoscrizione**.

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. Fai clic sul pulsante **Integrazioni** scheda . In Sincronizza con Salesforce, abilita la sincronizzazione notturna.

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. Seleziona il campo a cui desideri eseguire la sincronizzazione.

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | Campo | Descrizione |
   |---|---|
   | **Sincronizzazione con il campo Rinuncia Salesforce** | Selezionato per impostazione predefinita, aggiorna solo il campo Opt Out di Salesforce. |
   | **Campo Rinuncia alle vendite di Marketo** | Se desideri separare gli abbonamenti a vendite e marketing, scegli questa opzione per aggiornare gli altri [Campo Rinuncia alle vendite Marketo.](#msoo) |

## Installazione del campo Opt Out nel layout di pagina {#installing-the-opt-out-field-in-the-page-layout}

**Rifiuto e-mail**

L’opzione Rinuncia via e-mail è un campo standard di Salesforce che è disponibile per l’installazione da Salesforce. Devi essere un amministratore Salesforce per installarlo.

1. Vai a [Salesforce.com](https://salesforce.com) e accedi.

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. Fai clic sul tuo nome utente e seleziona **Configurazione**.

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. Nella casella di ricerca rapida cercare Contatto o Lead. In questo scenario si sta installando il campo nel layout della pagina Contatto, ma si desidera installare per entrambi i record persona.

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. Seleziona **Layout di pagina**.

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. Seleziona **Modifica** accanto al layout di pagina a cui si desidera aggiungere il campo.

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. Seleziona **Campi**.

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. Trascina e rilascia l’opzione Rinuncia via e-mail nel layout di pagina.

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. Fai clic su **Salva**.

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Rinuncia alle vendite Marketo {#marketo-sales-opt-out}

Il campo Rinuncia alle vendite Marketo è un campo personalizzato disponibile per gli utenti che hanno installato le personalizzazioni delle vendite Marketo.

Dopo aver installato con successo le personalizzazioni delle vendite Marketo in Salesforce vedrai il campo Rinuncia alle vendite Marketo disponibile.
