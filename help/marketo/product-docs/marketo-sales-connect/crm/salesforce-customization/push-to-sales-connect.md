---
unique-page-id: 14352477
description: Push to Sales Connect - Documentazione Marketo - Documentazione del prodotto
title: Invia a Sales Connect
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# Invia a Sales Connect {#push-to-sales-connect}

Il nostro pulsante Push to Tout (Invia a Tout) contiene un elenco dei lead/contatti in Salesforce e li inserisce in un gruppo in Sales Connect. Puoi quindi inviare rapidamente un’e-mail di gruppo personalizzabile con il tracciamento Tout allegato.

## Requisiti {#requirements}

* Pacchetto Salesforce Sales Connect installato dall&#39;amministratore Salesforce

* Pulsante Push to Sales Connect installato nella vista a elenco dall&#39;amministratore Salesforce

* Connessione Salesforce effettuata con Sales Connect per l’utente che effettua l’invio

## Procedura {#how-to}

1. Fai clic su **Lead/Contatto** in Salesforce.
1. Passa alla Vista a elenco da inviare a Sales Connect accanto al pulsante Vai.
1. Clic **Vai**.
1. Seleziona tutti i lead/contatti che desideri inviare al tout.
1. Seleziona **Invia a MSE**.
1. Verrà visualizzata una nuova finestra che verifica il numero di lead/contatti che desideri trasferire. Seleziona **Procedi al gruppo**. Sales Connect non invierà tramite push alcun contatto contrassegnato come Opt Out (Rifiuto) via e-mail in Salesforce o Unsubabbonamento in Sales Connect.

   >[!NOTE]
   >
   >Sales Connect aggiungerà questo gruppo denominato &quot;SFDC-...&quot; alla pagina Relazioni del [applicazione web](https://toutapp.com/login).

1. Seleziona **Invia intero gruppo tramite e-mail** per inviare l&#39;e-mail del gruppo.
