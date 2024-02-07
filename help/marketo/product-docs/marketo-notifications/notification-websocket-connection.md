---
description: Notifica - Connessione Websocket - Documentazione di Marketo - Documentazione del prodotto
title: Notifica - Connessione Websocket
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 94afeacfdecf71e6985daccc31dd67e3d19953ac
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---

# Notifica: connessione Websocket {#notification-websocket-connection}

Questo articolo è destinato agli utenti del Marketo Engage che hanno ricevuto la seguente notifica nella loro istanza di Marketo: `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are connected to now on March 3, 2024. Please work with your IT team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Se l&#39;utente o l&#39;organizzazione utilizza impostazioni restrittive per il firewall o il server proxy, potrebbe essere necessario inserire nell&#39;elenco Consentiti alcuni domini e intervalli di indirizzi IP per garantire il corretto funzionamento di Adobe Marketo Engage.

Il supporto Marketo non è configurato per l&#39;implementazione dei protocolli riportati di seguito. Se hai bisogno di assistenza, condividi questo articolo con il tuo team IT. Se limitano l’accesso web utilizzando un inserisco nell&#39;elenco Consentiti di, chiedi loro di aggiungere i seguenti domini (incluso l’asterisco) per consentire tutte le risorse Marketo e i websockets:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
