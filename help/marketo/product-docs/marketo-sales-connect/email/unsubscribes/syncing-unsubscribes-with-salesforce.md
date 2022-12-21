---
unique-page-id: 14746188
description: Sincronizzazione degli abbonamenti con Salesforce - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione degli abbonamenti con Salesforce
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Sincronizzazione degli abbonamenti con Salesforce {#syncing-unsubscribes-with-salesforce}

## Requisiti per l&#39;annullamento della sottoscrizione alla sincronizzazione con Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* Annulla sincronizzazione deve essere abilitato (per la sincronizzazione notturna)
* Il campo Opt Out deve essere installato in Salesforce
* I record personali in Sales Connect devono avere un ID Salesforce

**Annulla sottoscrizione push**

Quando un annullamento dell’abbonamento viene raccolto in Sales Connect, lo inviamo in tempo reale a Salesforce e aggiorniamo uno dei campi Opt Out con cui hai selezionato la sincronizzazione. Se hai disabilitato la sincronizzazione di Salesforce, l’annullamento della sottoscrizione verrà comunque inviato alla rinuncia all’e-mail.

**Annulla sincronizzazione**

Dopo aver attivato la sincronizzazione dell’annullamento dell’abbonamento (passaggio 3 qui sotto) verrà attivata la sincronizzazione notturna. La sincronizzazione avviene una volta al giorno intorno alle 20:00 PST. Sincronizza bidirezionale tutti gli annullamenti di abbonamenti in MSE/ToutApp con il campo Opt Out in Salesforce.

## Configurare Annulla sottoscrizione sincronizzazione con Salesforce {#configure-unsubscribe-sync-to-salesforce}

Gli utenti possono decidere se sincronizzare i propri annullamenti di abbonamenti con il campo Rifiuto e-mail standard con cui Marketo può anche eseguire la sincronizzazione, oppure possono sincronizzarsi con il campo Rinuncia alle vendite Marketo in modo che gli annullamenti di abbonamenti alle vendite e gli annullamenti di Marketing possano essere differenziati.

1. Vai a [applicazione web](https://toutapp.com/login), fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/one-1.png)

1. In Impostazioni amministratore, seleziona **Annulla sottoscrizione**.

   ![](assets/two-2.png)

1. Fai clic su **Sincronizzazione con Salesforce**, quindi attiva la sincronizzazione notturna.

   ![](assets/three-2.png)

1. Seleziona il campo a cui desideri eseguire la sincronizzazione.

   ![](assets/4.png)

   | Campo | Descrizione |
   |---|---|
   | **Sincronizzazione con il campo Rinuncia Salesforce** | Selezionato per impostazione predefinita, aggiorna solo il campo Opt Out di Salesforce. |
   | **Campo Rinuncia alle vendite di Marketo** | Se desideri separare gli abbonamenti a vendite e marketing, scegli questa opzione per aggiornare gli altri [Campo Rinuncia alle vendite Marketo.](#msoo) |

## Installazione del campo Opt Out nel layout di pagina {#installing-the-opt-out-field-in-the-page-layout}

**Rifiuto e-mail**

L’opzione Rinuncia via e-mail è un campo standard di Salesforce che è disponibile per l’installazione da Salesforce. Devi essere un amministratore Salesforce per installarlo.

1. Vai a [Salesforce.com](https://salesforce.com) e accedi.

   ![](assets/five-1.png)

1. Fai clic sul tuo nome utente e seleziona **Configurazione**.

   ![](assets/six-1.png)

1. Nella casella di ricerca rapida cercare Contatto o Lead. In questo scenario si sta installando il campo nel layout della pagina Contatto, ma si desidera installare per entrambi i record persona.

   ![](assets/seven-1.png)

1. Seleziona **Layout di pagina**.

   ![](assets/eight-1.png)

1. Seleziona **Modifica** accanto al layout di pagina a cui si desidera aggiungere il campo.

   ![](assets/nine.png)

1. Seleziona **Campi**.

   ![](assets/ten.png)

1. Trascina e rilascia l’opzione Rinuncia via e-mail nel layout di pagina.

   ![](assets/11.png)

1. Fai clic su **Salva**.

   ![](assets/twelve.png)

## Rinuncia alle vendite Marketo {#marketo-sales-opt-out}

Il campo Rinuncia alle vendite Marketo è un campo personalizzato disponibile per gli utenti che hanno installato le personalizzazioni di Marketo Sales Connect.

Dopo aver installato con successo le personalizzazioni di Marketo Sales Connect in Salesforce, verrà visualizzato il campo Rinuncia alle vendite Marketo disponibile.
