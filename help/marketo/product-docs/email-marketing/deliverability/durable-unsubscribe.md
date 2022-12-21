---
unique-page-id: 10094576
description: Annullamento dell’abbonamento a lungo termine - Documenti Marketo - Documentazione del prodotto
title: Annullamento durevole dell'abbonamento
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# Annullamento durevole dell&#39;abbonamento {#durable-unsubscribe}

Marketo ha migliorato il comportamento della funzionalità di annullamento dell’abbonamento per renderla &quot;durevole&quot;. Abbiamo aggiunto uno stato e-mail principale, separato dal flag di annullamento dell’abbonamento visibile nel record di dettaglio della persona.

Se il flag di annullamento dell’abbonamento è impostato su false per true, lo stato dell’e-mail principale viene aggiornato e la modifica viene propagata ad altre persone con lo stesso indirizzo e-mail. Se una persona viene rimossa e ricreata, o se viene creato un nuovo record con lo stesso indirizzo e-mail, il flag di annullamento dell’abbonamento **not** essere sovrascritti.

>[!NOTE]
>
>L&#39;annullamento della sottoscrizione durevole funziona su tutte le partizioni nell&#39;intero database Marketo.

## Aggiorna il flag Annulla sottoscrizione da True a False (ad esempio, Re-iscrivi una persona) {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Ci sono diversi modi in cui una persona può essere riabbonata.

A Salesforce, **cancella** campo Rinuncia via e-mail nel record del lead/contatto. Verrà eseguita la sincronizzazione con Marketo.

![](assets/one.png)

In Marketo, **cancella** la casella di cui annullare l’iscrizione nella scheda Informazioni del record della persona.

![](assets/two.png)

Eseguire un **Modifica valore dati** passaggio di flusso come mostrato di seguito su una o più persone.

![](assets/three.png)

Aggiornare una persona esistente tramite API SOAP.

## Creazione di una nuova persona {#creating-a-new-person}

Quando viene creata una nuova persona, Marketo la confronta con la tabella di stato dell’e-mail principale. Se la persona è stata precedentemente annullata, verrà aggiornato il record per annullare l’abbonamento.

## Modifica di un indirizzo e-mail {#changing-an-email-address}

Se modifichi l’indirizzo e-mail di una persona in un indirizzo e-mail non iscritto, tale persona verrà cancellata dall’abbonamento. Questa modifica può verificarsi in Marketo o Salesforce.

Se cambi un indirizzo e-mail non iscritto a uno che è iscritto, la persona verrà abbonata.

## Nuova sottoscrizione {#re-subscribing}

Proprio come un annullamento dell’abbonamento farebbe sì che tutte le persone con lo stesso indirizzo e-mail venissero cancellate, un nuovo abbonamento infatti avrebbe fatto sì che ogni persona avesse lo stesso indirizzo e-mail.

## Registro attività {#activity-log}

Definizioni di modifica del valore dei dati per _updateLeadEmailStatus_ e _resetLeadEmailStatus_ si trova in [presente articolo comunitario](https://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688).

>[!MORELIKETHIS]
>
>[Informazioni sull’annullamento della sottoscrizione](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
