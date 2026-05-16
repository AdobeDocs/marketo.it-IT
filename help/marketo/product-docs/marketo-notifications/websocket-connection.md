---
description: Dettagli della notifica per gli utenti di Marketo Engage che hanno ricevuto la notifica Impossibile stabilire una connessione Websocket
title: Notifica - Connessione Websocket
hide: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
TQID: https://experienceleague.adobe.com/NpcRnxQPi03CF8z77Urrfs2P2phkuRbh2pd5J1UquFk
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 123
ht-degree: 30%

---

# Notifica: connessione Websocket {#notification-websocket-connection}

Questo documento è destinato agli utenti di Marketo Engage che hanno ricevuto la seguente notifica nella loro istanza di Marketo: `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Se tu o la tua organizzazione utilizzate impostazioni restrittive per il firewall o il server proxy, tu o l’amministratore della rete potreste dover inserire nell’elenco Consentiti alcuni domini e intervalli di indirizzi IP per garantire il corretto funzionamento di Adobe Marketo Engage.

Il supporto Marketo non è configurato per l&#39;implementazione dei protocolli riportati di seguito. Se hai bisogno di assistenza, condividi questo documento con il tuo team IT. Se limitano l’accesso web utilizzando un inserisco nell&#39;elenco Consentiti di, chiedi loro di aggiungere i seguenti domini (incluso l’asterisco) per consentire tutte le risorse Marketo e i websockets:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
