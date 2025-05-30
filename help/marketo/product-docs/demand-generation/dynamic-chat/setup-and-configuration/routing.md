---
description: Indirizzamento - Documentazione Marketo - Documentazione del prodotto
title: Indirizzamento
feature: Dynamic Chat
exl-id: e20193b9-55c1-40f2-9e42-5b5dc9b88144
source-git-commit: 19f7a38a6a87bc66084e7e45f5bf49cd0d29c3cd
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Indirizzamento {#routing}

Le riunioni prenotate in Dynamic Chat possono essere instradate in due modi. Round robin o utilizzo di una regola personalizzata.

Round robin: le riunioni vengono assegnate agli agenti in sequenza. Quindi se hai cinque agenti e l&#39;agente tre ha preso l&#39;ultima riunione, l&#39;agente quattro prenderà la prossima, seguita dall&#39;agente cinque, e poi di nuovo dall&#39;agente uno.

Regola personalizzata: è possibile scegliere agenti specifici per ricevere riunioni in base agli attributi selezionati.

>[!NOTE]
>
>All’Instradamento dell’account viene assegnata la priorità più elevata. Quando un visitatore raggiunge il punto della conversazione per prenotare una riunione o avviare una chat in tempo reale, [Instradamento account](#account-routing) viene controllato prima di prendere in considerazione altre opzioni di instradamento.

## Creare una regola personalizzata {#create-a-custom-rule}

In questo esempio invieremo tutte le riunioni dagli stati dedotti di CA, OR e WA all&#39;agente John.

1. In Configurazione fare clic su **Regole di routing**.

   ![](assets/routing-1.png)

1. Per impostazione predefinita, viene aperta la scheda **Regole personalizzate**.

   ![](assets/routing-2.png)

1. Fai clic su **Crea regola**.

   ![](assets/routing-3.png)

1. Denomina la regola. Facoltativamente, puoi aggiungere una descrizione e impostarne il livello di priorità. Fai clic su **Avanti**.

   ![](assets/routing-4.png)

1. Scegli gli agenti desiderati.

   ![](assets/routing-5.png)

1. Trascina sull’attributo o sugli attributi desiderati.

   ![](assets/routing-6.png)

1. Trova e seleziona i valori desiderati.

   ![](assets/routing-7.png)

1. Dopo aver selezionato tutti i valori desiderati, fare clic su **Salva**.

   ![](assets/routing-8.png)

## Indirizzamento account {#account-routing}

Identifica e carica il tuo account di destinazione e i rispettivi proprietari delle vendite e indirizza i visitatori provenienti da tali account direttamente al rispettivo proprietario dell’account.

![](assets/routing-9.png)

>[!PREREQUISITES]
>
>Prima che l&#39;instradamento dell&#39;account _Account_ sia visibile in Dynamic Chat, è necessario abilitare le autorizzazioni in Admin Console. Vedi [Abilita autorizzazioni](#enable-permissions) di seguito.

### Abilita autorizzazioni {#enable-permissions}

+++ Abilita autorizzazioni di indirizzamento degli account

1. Accedi a [https://adminconsole.adobe.com/](https://adminconsole.adobe.com/){target="_blank"}.

1. In _Prodotti_, seleziona **Dynamic Chat**.

   ![](assets/routing-10.png)

1. In _Profili di prodotto_, selezionare il profilo desiderato.

   ![](assets/routing-11.png)

1. Fare clic sulla scheda **Autorizzazioni**.

   ![](assets/routing-12.png)

1. Fai clic sull&#39;icona Modifica (![icona Modifica](assets/icon-routing-edit.png)) accanto a _Configurazione_.

   ![](assets/routing-13.png)

1. Fai clic sul segno **+** accanto a _Visualizza indirizzamento account_.

   ![](assets/routing-14.png){width="600" zoomable="yes"}

1. Al termine, fai clic su **Salva**.

+++

### Aggiungi un account {#add-an-account}

In questo esempio, indirizzeremo tutti i dipendenti della Lego direttamente all&#39;agente Steven.

1. Nella scheda Instradamento account, fare clic su **+ Aggiungi account**.

   ![](assets/routing-15.png)

   >[!TIP]
   >
   >Puoi creare più account contemporaneamente facendo clic su **Carica elenco account** e caricando un file CSV.

1. Immetti il nome della società, il dominio e seleziona l’agente desiderato.

   ![](assets/routing-16.png)
