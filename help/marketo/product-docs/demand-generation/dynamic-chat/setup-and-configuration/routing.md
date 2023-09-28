---
description: Indirizzamento - Documentazione Marketo - Documentazione del prodotto
title: Indirizzamento
feature: Dynamic Chat
exl-id: 93d1a96d-c101-4a1c-898c-dcadb5cdce85
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 1%

---

# Indirizzamento {#routing}

Le riunioni prenotate in Dynamic Chat possono essere instradate in due modi. Round robin o utilizzo di una regola personalizzata.

Round robin: le riunioni vengono assegnate agli agenti in sequenza. Quindi se hai cinque agenti e l&#39;agente tre ha preso l&#39;ultima riunione, l&#39;agente quattro prenderà la prossima, seguita dall&#39;agente cinque, e poi di nuovo dall&#39;agente uno.

Regola personalizzata: è possibile scegliere agenti specifici per ricevere riunioni in base agli attributi selezionati.

>[!NOTE]
>
>All’Instradamento dell’account viene assegnata la priorità più elevata. Quando un visitatore raggiunge il punto della conversazione per prenotare una riunione o avviare una chat in tempo reale, [Indirizzamento account](#account-routing) viene selezionato prima di prendere in considerazione altre opzioni di instradamento.

## Creare una regola personalizzata {#create-a-custom-rule}

In questo esempio invieremo tutte le riunioni dagli stati dedotti di CA, OR e WA all&#39;agente John.

1. In Configurazione, fai clic su **Regole di instradamento**.

   ![](assets/routing-1.png)

1. Fai clic su **Regole personalizzate** scheda.

   ![](assets/routing-2.png)

1. Clic **Crea regola**.

   ![](assets/routing-3.png)

1. Denomina la regola. Facoltativamente, puoi aggiungere una descrizione e impostarne il livello di priorità. Fai clic su **Avanti**.

   ![](assets/routing-4.png)

1. Scegli gli agenti desiderati.

   ![](assets/routing-5.png)

1. Trascina sull’attributo o sugli attributi desiderati.

   ![](assets/routing-6.png)

1. Trova e seleziona i valori desiderati.

   ![](assets/routing-7.png)

1. Dopo aver selezionato tutti i valori desiderati, fai clic su **Salva**.

   ![](assets/routing-8.png)

## Indirizzamento account {#account-routing}

Identifica e carica il tuo account di destinazione e i rispettivi proprietari delle vendite e indirizza i visitatori provenienti da tali account direttamente al rispettivo proprietario dell’account.

![](assets/routing-9.png)

### Aggiungi un account {#add-an-account}

In questo esempio, indirizzeremo tutti i dipendenti della Lego direttamente all&#39;agente Steven.

1. Nella scheda Instradamento account fare clic su **+ Aggiungi account**.

   ![](assets/routing-10.png)

   >[!TIP]
   >
   >Puoi creare più account contemporaneamente facendo clic su **Carica elenco account** e il caricamento di un file CSV.

1. Immetti il nome della società, il dominio e seleziona l’agente desiderato.

   ![](assets/routing-11.png)
