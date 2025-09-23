---
description: Gestione degli agenti - Documentazione di Marketo - Documentazione del prodotto
title: Gestione agente
feature: Dynamic Chat
exl-id: 151d8cf2-a5b7-43c4-8418-cc22252108b2
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 2%

---

# Gestione agente {#agent-management}

In Gestione agenti, visualizza un elenco di agenti nell’istanza Dynamic Chat, gestisci i team e imposta le regole di fallback.

![](assets/agent-management-1.png)

## Agenti {#agents}

Questa scheda elenca tutti gli agenti nell’istanza di Dynamic Chat e include informazioni quali nome, indirizzo e-mail, stato della chat in tempo reale e altro ancora.

![](assets/agent-management-2.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Non trovi un agente _appena_ aggiunto? Potrebbero essere necessarie fino a due ore prima che vengano visualizzate qui dopo essere state aggiunte nell’Admin Console di Adobe.

## Team {#teams}

Gli amministratori possono creare team di agenti per facilitare l’inoltro a gruppi specifici di agenti di vendita.

>[!AVAILABILITY]
>
>L’accesso a Teams richiede un abbonamento a Dynamic Chat Prime. Per ulteriori informazioni, contatta il team dell’account di Adobe (il tuo Account Manager).

![](assets/agent-management-3.png)

### Creare un team {#create-a-team}

1. Fare clic su **+ Crea team**.

   ![](assets/agent-management-4.png)

1. Dai un nome alla tua squadra.

   ![](assets/agent-management-5.png)

1. Fare clic sul menu a discesa **Aggiungi agenti** e selezionare gli agenti desiderati.

   ![](assets/agent-management-6.png)

1. Fai clic su **Crea**.

   ![](assets/agent-management-7.png)

## Regole di fallback {#fallback-rules}

### Fallback riunione {#meeting-fallback}

Selezionare un messaggio standard (di sistema) o scriverne uno personalizzato che i visitatori possano visualizzare quando la prenotazione della riunione non è disponibile.

![](assets/agent-management-8.png)

### Fallback chat in diretta {#live-chat-fallback}

Seleziona un messaggio standard (di sistema) o scrivine uno personalizzato che i visitatori visualizzino quando la chat in diretta non è disponibile.

![](assets/agent-management-9.png)

>[!NOTE]
>
>* Se si seleziona la casella di controllo _Includi opzione prenotazione riunioni_, il visitatore della chat potrà prenotare una riunione quando non sono disponibili agenti per la chat in diretta.
>
>* **Per qualsiasi regola/team personalizzato come scheda di chat in diretta**: durante la verifica degli agenti, se non sono disponibili o non sono in grado di connettersi, verrà eseguito il fallback su Round Robin per cercare &quot;Agenti disponibili&quot; (tutti gli agenti disponibili in quel momento, indipendentemente dalla logica/regola di routing inserita nel flusso).

>[!TIP]
>
>Durante la creazione di un messaggio personalizzato, puoi applicare uno stile al font, utilizzare i collegamenti e persino inserire emoji. `:)`
