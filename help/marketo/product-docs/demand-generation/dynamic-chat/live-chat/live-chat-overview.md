---
description: Panoramica della chat in diretta - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica chat in diretta
feature: Dynamic Chat
exl-id: 44e8b249-b534-4cec-a612-daa184acd266
source-git-commit: 870dd6df82c605fffa6681d68867354084988bcd
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Panoramica chat in diretta {#live-chat-overview}

La chat in tempo reale consente ai visitatori del sito web di intrattenere conversazioni in chat in tempo reale con i tuoi agenti di vendita.

## Aggiungi agenti chat in tempo reale {#add-live-chat-agents}

Per iniziare a utilizzare la chat in diretta, devi aggiungere i tuoi agenti chat in diretta come [utenti in Adobe Admin Console](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} and give them the [Live Chat permission](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. Al termine dell’operazione, puoi aggiungere una [scheda chat in diretta](#using-the-live-chat-card) in una finestra di dialogo nuova o esistente.

Quando i visitatori richiedono di chattare con un agente tramite la tua finestra di dialogo, gli agenti avranno più [opzioni di notifica](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. When they click on the notification, they'll be taken to their [Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} dove possono iniziare a chattare con il visitatore.

>[!NOTE]
>
>L’avatar dell’agente live utilizza l’immagine del profilo dell’account Adobe dell’agente. Per aggiornare l&#39;immagine, segui [questi passaggi](https://helpx.adobe.com/manage-account/using/edit-adobe-account-personal-profile.html){target="_blank"}.

## Utilizzo della scheda Live Chat {#using-the-live-chat-card}

Utilizza la scheda della chat in tempo reale in [Progettazione flussi](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"} quando desideri che i visitatori chattino con un agente live.

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>La scheda della chat in diretta deve essere sempre l’ultima scheda del ramo. Se la scheda viene posizionata in un punto casuale nel ramo, potrebbe sorprendere il visitatore collegandolo improvvisamente a un agente.

### Best practice {#best-practices}

* Utilizza una scheda domande prima della scheda chat in diretta in cui si chiede al visitatore se desidera connettersi.
* Una volta che il visitatore accetta di connettersi, utilizza la scheda di acquisizione delle informazioni per raccogliere alcune delle sue informazioni, come nome/cognome, indirizzo e-mail, qualifica professionale, ecc. (si consiglia di richiedere almeno nome e indirizzo e-mail).

## Opzioni scheda chat in diretta {#live-chat-card-options}

Facendo clic sulla scheda della chat dal vivo nel flusso, puoi scegliere come indirizzare il visitatore. Scegli tra round robin, un agente, regole personalizzate o un team.

![](assets/live-chat-overview-2.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>Round robin</b></td>
   <td>Le chat vengono assegnate agli agenti in ordine sequenziale.</td>
  </tr> 
  <tr> 
   <td><b>Agente</b></td>
   <td>Scegli un agente specifico per ricevere la chat.</td>
  </tr>
    <tr> 
   <td><b>Regole personalizzate</b></td>
   <td>Tutte le regole personalizzate vengono esaminate ogni volta che si considera dove indirizzare il visitatore. Se il visitatore non è idoneo per alcuna regola personalizzata, ottiene il <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">messaggio di fallback di live chat</a>.</td>
  </tr> 
  <tr> 
   <td><b>Team</b></td>
   <td>Scegli un team specifico per ricevere la chat. Se questa opzione è selezionata, verrà assegnato round robin all'interno del team.</td>
  </tr>
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Casella in entrata agente](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
