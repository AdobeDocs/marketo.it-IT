---
description: Notifica - Connessione Websocket - Documentazione di Marketo - Documentazione del prodotto
title: Notifica - Connessione Websocket
hide: true
hidefromtoc: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
source-git-commit: eb3e7983f7521d025dff1f5d79b8caeaeb0f622c
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---

# Notifica: connessione Websocket {#notification-websocket-connection}

Questo documento è destinato agli utenti del Marketo Engage che hanno ricevuto la seguente notifica nella loro istanza Marketo: `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Se l&#39;utente o l&#39;organizzazione utilizza impostazioni restrittive del firewall o del server proxy, potrebbe essere necessario inserire nell&#39;elenco Consentiti alcuni domini e intervalli di indirizzi IP per garantire il corretto funzionamento di Adobe Marketo Engage.

Il supporto Marketo non è configurato per l&#39;implementazione dei protocolli riportati di seguito. Se hai bisogno di assistenza, condividi questo documento con il tuo team IT. Se limitano l’accesso web utilizzando un inserisco nell&#39;elenco Consentiti di, chiedi loro di aggiungere i seguenti domini (incluso l’asterisco) per consentire tutte le risorse Marketo e i websockets:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
