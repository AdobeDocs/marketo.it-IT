---
unique-page-id: 10094576
description: Annullamento duraturo dell’abbonamento - Documentazione di Marketo - Documentazione del prodotto
title: Annullare l’iscrizione durevole
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 1%

---

# Annullare l’iscrizione durevole {#durable-unsubscribe}

Marketo ha migliorato il comportamento della funzionalità di annullamento dell’abbonamento per renderla &quot;durevole&quot;. È stato aggiunto lo stato di un’e-mail principale, separato dal flag di annullamento dell’iscrizione visibile nel record dei dettagli della persona.

Se il flag di annullamento dell’iscrizione è impostato su false su true, lo stato dell’e-mail principale viene aggiornato e la modifica viene propagata ad altre persone con lo stesso indirizzo e-mail. Se una persona viene rimossa e ricreata o se viene creato un nuovo record con lo stesso indirizzo e-mail, il flag di annullamento dell&#39;iscrizione **non** verrà sovrascritto.

>[!NOTE]
>
>L’annullamento dell’abbonamento durevole funziona su tutte le partizioni dell’intero database di Marketo.

## Aggiorna il flag di annullamento iscrizione da True a False (ad esempio, rinnova l’iscrizione di una persona) {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

È possibile effettuare nuovamente l’abbonamento in diversi modi.

In Salesforce, cancella il campo Rinuncia e-mail nel record del lead/contatto. Verrà eseguita la sincronizzazione con Marketo.

![Schermata Salesforce](assets/durable-unsubscribe-1.png)

In Marketo, deseleziona la casella di annullamento dell’abbonamento nella scheda Info del record dell’utente.

![Cancellazione della casella di annullamento dell&#39;iscrizione in un record persona](assets/durable-unsubscribe-2.png)

Esegui un passaggio del flusso _Modifica valore dati_ come mostrato di seguito per una o più persone.

![Passaggio del flusso del valore dei dati di modifica](assets/durable-unsubscribe-3.png)

## Creazione di una nuova persona {#creating-a-new-person}

Quando viene creata una nuova persona, Marketo la confronta con la tabella dello stato dell’e-mail principale. Se la persona ha annullato l’abbonamento in precedenza, il record verrà aggiornato in modo da annullare l’abbonamento.

## Modifica di un indirizzo e-mail {#changing-an-email-address}

Se modifichi l’indirizzo e-mail di una persona impostandolo su un indirizzo e-mail a cui non è stata effettuata l’iscrizione, la persona verrà annullata. Questa modifica può verificarsi in Marketo o [!DNL Salesforce].

## Ri-iscrizione {#re-subscribing}

Proprio come un annullamento dell’iscrizione causerebbe la cancellazione di tutte le persone con lo stesso indirizzo e-mail, un nuovo abbonamento comporterebbe in realtà la reiscrizione di ogni persona con lo stesso indirizzo e-mail.

>[!MORELIKETHIS]
>
>[Informazioni sull&#39;annullamento dell&#39;iscrizione](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
