---
description: Funzioni di callback - Documentazione di Marketo - Documentazione del prodotto
title: Funzioni callback
feature: Dynamic Chat
exl-id: 5ae7f6cb-5c57-4257-8a1a-992c9602cfaa
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 3%

---

# Funzioni callback {#callback-functions}

Puoi utilizzare le funzioni di callback del widget Dynamic Chat per inviare eventi di conversazione a qualsiasi piattaforma di terze parti.

## Guida introduttuva {#getting-started}

Questo evento indica che il widget Dynamic Chat è pronto per l&#39;uso e viene attivato quando tutti gli script relativi a Dynamic Chat vengono caricati nella pagina Web.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    // code here will execute when chatbot scripts are loaded in a webpage
});
```

## Eventi di conversazione {#conversation-events}

Questi eventi sono correlati a una conversazione con targeting su una pagina specifica per un visitatore specifico.

### Conversazione attivata

Viene risolta una conversazione (ad esempio, un dialogo) destinata a un visitatore del sito web e viene mostrato il chatbot.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => {
 // code here will execute when the chatbot is loaded for a visitor
    });
});
```

### Conversazione coinvolta {#conversation-engaged}

Il visitatore ingaggiato (ad esempio, ha fornito la sua prima risposta) con il chatbot.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_ENGAGED, (event) => {
 // code here will execute when a visitor engages with the chatbot
     });
});
```

### Conversazione completata {#conversation-completed}

Il visitatore ha raggiunto la fine della conversazione.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_COMPLETED, (event) => {
 // code here will execute when a conversation is completed
     });
});
```

### Conversazione chiusa

Il visitatore ha chiuso la conversazione prima di raggiungere la fine.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_CLOSED, (event) => {
 // code here will execute when a conversation is closed
    });
});
```

Il parametro `event` è un oggetto con metadati relativi alla conversazione. È possibile accedere a questi metadati accedendo a `event.data`.

Di seguito sono riportati alcuni valori di metadati chiave a cui è possibile accedere:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadati</th>
    <th style="width:25%">Attributi</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nome conversazione</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>ID conversazione</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Tipo di conversazione (flusso di conversazione)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Tipo di interfaccia utente (popup/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>ID sessione</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## Eventi di input visitatore

Questi eventi vengono attivati quando un visitatore che partecipa a una conversazione fornisce le sue informazioni di contatto (ad esempio, numero di telefono o indirizzo e-mail). Di seguito sono riportati gli eventi che rientrano in questa categoria.

### Numero di telefono {#phone-number}

Questo evento viene attivato quando un visitatore fornisce il proprio numero di telefono durante la conversazione.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_INPUT_PHONE, (event) => {
 // code here will execute when a visitor provides their phone number
    });
});
```

### ID e-mail {#email-id}

Questo evento viene attivato quando un visitatore fornisce il proprio indirizzo e-mail durante la conversazione.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_INPUT_EMAIL, (event) => {
 // code here will execute when a visitor provides their email address
    });
});
```

Il parametro `event` è un oggetto con metadati relativi alla conversazione. È possibile accedere a questi metadati accedendo a `event.data`.

Di seguito sono riportati alcuni valori di metadati chiave a cui è possibile accedere:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadati</th>
    <th style="width:25%">Attributi</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nome conversazione</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>ID conversazione</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Tipo di conversazione (flusso di conversazione)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Tipo di interfaccia utente (popup/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>ID sessione</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## Meeting Booking Events {#meeting-booking-events}

Questi eventi vengono attivati quando un visitatore registra una riunione con il tuo rappresentante commerciale.

Di seguito sono riportati gli eventi che rientrano in questa categoria.

### Riunione prenotata {#meeting-booked}

Questo evento viene attivato quando un visitatore registra una riunione nel calendario di un agente.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_MEETING_BOOKED, (event) => {
 // code here will execute when a meeting is booked
    });
});
```

Il parametro `event` è un oggetto con metadati relativi alla conversazione. È possibile accedere a questi metadati accedendo a `event.data`.

Di seguito sono riportati alcuni valori di metadati chiave a cui è possibile accedere:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadati</th>
    <th style="width:25%">Attributi</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nome conversazione</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>ID conversazione</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Tipo di conversazione (flusso di conversazione)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Tipo di interfaccia utente (popup/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>ID sessione</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>Nome agente</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>ID agente</td>
    <td>payload.agentID</td>
  </tr>
  <tr>
    <td>Informazioni riunione</td>
    <td>payload.meetingInfo</td>
  </tr>
</tbody>
</table>

## Eventi chat in diretta {#live-chat-events}

Questi eventi vengono attivati quando un visitatore si connette con un agente live durante il suo coinvolgimento con il chatbot.

Di seguito sono riportati gli eventi che rientrano in questa categoria.

### Richiesta chat in diretta {#live-chat-requested}

Questo evento viene attivato quando un visitatore seleziona l’opzione per chattare con un agente live e un agente disponibile viene risolto.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUESTED, (event) => {
 // code here will execute when a visitor requests a live chat
    });
});
```

### Chat in tempo reale avviata {#live-chat-initiated}

Questo evento viene attivato quando un visitatore seleziona l’opzione per chattare con un agente live e un agente accetta la chat.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_INITIATED, (event) => {
 // code here will execute after a live agent accepts the chat
    });
});
```

### Chat in tempo reale terminata {#live-chat-ended}

Questo evento viene attivato al termine di una conversazione tra un visitatore e l’agente live.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_ENDED, (event) => {
 // code here will execute when a live chat is ended
    });
});
```

### Timeout chat in tempo reale {#live-chat-timeout}

Questo evento viene attivato quando una conversazione live chat scade perché il visitatore non risponde più o perché il visitatore non risponde più.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUEST_TIMEOUT, (event) => {
 // code here will execute when a visitor abandons a live chat
    });
});
```

Il parametro `event` è un oggetto con metadati relativi alla conversazione. È possibile accedere a questi metadati accedendo a `event.data`.

Di seguito sono riportati alcuni valori di metadati chiave a cui è possibile accedere:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadati</th>
    <th style="width:25%">Attributi</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nome conversazione</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>ID conversazione</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Tipo di conversazione (flusso di conversazione)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Tipo di interfaccia utente (popup/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>ID sessione</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>Nome agente</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>ID agente</td>
    <td>payload.agentID</td>
  </tr>
</tbody>
</table>

Se desideri inviare uno di questi eventi a una piattaforma di analisi come Adobe Analytics o Google Analytics, devi aggiungere la rispettiva chiamata di tracciamento all&#39;interno di questi eventi Dynamic Chat. Avrebbe un aspetto simile all’esempio di seguito.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => {
 // Enter Adobe Analytics or Google Analytics function here
    ga('send', 'event', {
      eventCategory: Dynamic Chat Conversations',
      eventAction: 'Conversation Triggered',
      eventLabel: event.data.payload.id,
    });
    });
});
```
