---
unique-page-id: 10094576
description: Durable Unsubscription - Marketo Docs - Documentazione del prodotto
title: Annullamento della sottoscrizione
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---


# Annullamento sottoscrizione duratura {#durable-unsubscribe}

Marketo ha migliorato il comportamento della funzionalità di annullamento della sottoscrizione per renderla &quot;durevole&quot;. Abbiamo aggiunto uno stato e-mail principale, separato dal flag di annullamento della sottoscrizione visibile nel record dei dettagli della persona.

Se il flag di annullamento della sottoscrizione è impostato su false, lo stato dell’e-mail principale viene aggiornato e la modifica viene propagata ad altre persone con lo stesso indirizzo e-mail. Se una persona viene rimossa e ricreata, o se viene creato un nuovo record con lo stesso indirizzo e-mail, il flag di annullamento della sottoscrizione sarà **non** sovrascritto.

>[!NOTE]
>
>Durable Unsubscription funziona su tutte le partizioni nell&#39;intero database Marketo.

## Aggiorna il flag di annullamento della sottoscrizione da True a False (ad esempio, Re-iscrivi a Person) {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Ci sono diversi modi in cui una persona può essere riscritta.

In Salesforce, **cancellare** il campo Rifiuto e-mail nel record del lead/contatto. Questa operazione verrà sincronizzata con Marketo.

![](assets/one.png)

In Marketo, **deselezionare** la casella non sottoscritta nella scheda Informazioni del record della persona.

![](assets/two.png)

Eseguire un passaggio di flusso **Change Data Value** come mostrato di seguito su uno o più utenti.

![](assets/three.png)

Aggiornare una persona esistente tramite API SOAP.

## Creazione di una nuova persona {#creating-a-new-person}

Quando viene creata una nuova persona, Marketo la verifica rispetto alla tabella di stato delle e-mail principale. Se la persona è stata precedentemente annullata la sottoscrizione, il record verrà aggiornato in modo da annullare la sottoscrizione.

## Modifica di un indirizzo e-mail {#changing-an-email-address}

Se cambiate l’indirizzo e-mail di una persona impostandolo su un indirizzo e-mail non iscritto, tale persona verrà cancellata dall’iscrizione. Questa modifica può avvenire in Marketo o Salesforce.

Se cambiate l’indirizzo e-mail di un utente che non ha effettuato l’iscrizione, tale utente verrà registrato.

## Iscrizione di nuovo {#re-subscribing}

Così come un annullamento dell’iscrizione causerebbe l’annullamento dell’iscrizione a tutti gli utenti con lo stesso indirizzo e-mail, un nuovo abbonamento infatti richiederebbe l’iscrizione a ogni utente con lo stesso indirizzo e-mail.

## Registro attività {#activity-log}

Le definizioni di modifica del valore dei dati per _updateLeadEmailStatus_ e _resetLeadEmailStatus_ sono disponibili in [questo articolo della community](https://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688).

>[!MORELIKETHIS]
>
>[Informazioni su Annulla sottoscrizione](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
