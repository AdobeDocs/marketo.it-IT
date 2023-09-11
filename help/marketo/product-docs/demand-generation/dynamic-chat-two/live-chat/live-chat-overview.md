---
description: Panoramica della chat in diretta - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica chat in diretta
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 863e5e542e2006ee15f44ad949e876e56a9b39e3
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 2%

---

# Panoramica chat in diretta {#live-chat-overview}

Utilizza la scheda della chat in tempo reale in [stream designer](/help/marketo/product-docs/demand-generation/dynamic-chat-two/automated-chat/stream-designer.md){target="_blank"} quando desideri che i visitatori chattino con un agente live.

## Utilizzo della scheda Live Chat {#using-the-live-chat-card}

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>La scheda della chat in diretta deve essere sempre l’ultima scheda del ramo. Se la scheda viene posizionata in un punto casuale nel ramo, potrebbe sorprendere il visitatore collegandolo improvvisamente a un agente.

**Best practice**

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
   <td>Tutte le regole personalizzate vengono esaminate ogni volta che si considera dove indirizzare il visitatore. Se il visitatore non soddisfa nessuno dei criteri, eseguirà una REGOLA DI FALLBACK???</td>
  </tr> 
  <tr> 
   <td><b>Team</b></td>
   <td>Scegli un team specifico per ricevere la chat. Se questa opzione è selezionata, verrà assegnato round robin all'interno del team.</td>
  </tr>
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>* [Casella in entrata agente](/help/marketo/product-docs/demand-generation/dynamic-chat-two/live-chat/agent-inbox.md){target="_blank"}
>* [Notifiche](/help/marketo/product-docs/demand-generation/dynamic-chat-two/live-chat/notifications.md){target="_blank"}
