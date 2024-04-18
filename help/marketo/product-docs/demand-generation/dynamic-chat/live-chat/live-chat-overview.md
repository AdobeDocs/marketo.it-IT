---
description: Panoramica della chat in diretta - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica chat in diretta
feature: Dynamic Chat
exl-id: 44e8b249-b534-4cec-a612-daa184acd266
source-git-commit: 14ccfe39059b9c900a5e5e00b082146bb500d79d
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# Panoramica chat in diretta {#live-chat-overview}

La chat in tempo reale consente ai visitatori del sito web di intrattenere conversazioni in chat in tempo reale con i tuoi agenti di vendita.

>[!NOTE]
>
>Per coloro che fanno parte del pacchetto di selezione del Dynamic Chat, la chat in diretta è una funzione di prova con un limite di durata di 100 engagement. Quando questo limite viene raggiunto, tutti i visitatori che richiedono di chattare con un agente live non saranno connessi e riceveranno invece il messaggio di fallback globale. Per aumentare il limite, contatta il rappresentante del tuo account Adobe per discutere le opzioni di aggiornamento del pacchetto.

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

## Notifiche chat in diretta {#live-chat-notifications}

>[!IMPORTANT]
>
>Per ricevere le notifiche del browser per la chat in tempo reale, tutti gli agenti chat in tempo reale devono abilitare le notifiche del browser per il Dynamic Chat quando richiesto.

### Abilitazione delle notifiche {#enabling-notifications}

Gli agenti di chat live visualizzeranno un banner nella parte superiore dello schermo quando effettuano l’accesso che recita &quot;Abilita le notifiche del browser per ricevere le notifiche di chat live&quot;. Clic **Abilita**.

![](assets/live-chat-overview-4.png)

Agli agenti di chat live verrà quindi richiesto dal browser di visualizzare le notifiche. Clic **Consenti**.

![](assets/live-chat-overview-5.png)

Se gli agenti non ricevono le notifiche del browser anche dopo averlo consentito nel browser, potrebbe essere necessario abilitare le notifiche per il browser nelle impostazioni di notifica del sistema operativo:

[Passaggi per Mac](https://support.apple.com/guide/mac-help/change-notifications-settings-mh40583/mac){target="_blank"}

[Passaggi per Windows](https://support.microsoft.com/en-us/windows/change-notification-settings-in-windows-8942c744-6198-fe56-4639-34320cf9444e){target="_blank"}

### Quando una chat in diretta viene indirizzata a un agente {#when-a-live-chat-is-routed-to-an-agent}

Quando una chat in diretta viene indirizzata a un agente, vede un banner blu nella parte superiore dello schermo che chiede di accettare.

![](assets/live-chat-overview-3.png)

>[!TIP]
>
>Puoi anche impostare le notifiche del browser, che ti invieranno un avviso nel caso in cui non sia stato effettuato l’accesso al Dynamic Chat.
>
>* Abilitare le notifiche del browser in [Google Chrome](https://support.google.com/chrome/answer/3220216?hl=en&amp;co=GENIE.Platform%3DDesktop){target="_blank"}
>* Abilitare le notifiche del browser in [Mozilla Firefox](https://support.mozilla.org/en-US/kb/push-notifications-firefox){target="_blank"}

### Aspetti da considerare {#things-to-note}

* Gli agenti hanno 45 secondi di tempo per rispondere prima che venga visualizzato il messaggio &quot;Accept chat&quot; (Accetta chat). Successivamente, i visitatori riceveranno la [messaggio di fallback](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback){target="_blank"}. Per gli abbonati Dynamic Chat Prime che hanno l’opzione di indirizzamento impostata su **Team**, verrà tentato un altro agente prima che venga visualizzato il messaggio di fallback.
* Al momento esiste un limite di 10 chat live per agente.

>[!MORELIKETHIS]
>
>[Casella in entrata agente](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
