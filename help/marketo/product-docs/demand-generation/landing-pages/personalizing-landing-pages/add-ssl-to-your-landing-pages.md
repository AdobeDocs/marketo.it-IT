---
unique-page-id: 2359828
description: Aggiungere SSL alle pagine di destinazione - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere SSL alle pagine di destinazione
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: d5993d7c638994ea93446d20cbd1f1ae0b25e622
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---

# Aggiungere SSL alle pagine di destinazione {#add-ssl-to-your-landing-pages}

La crittografia SSL (Secure Socket Layer) consente di rendere sicure tutte le pagine di destinazione di un’istanza del Marketo Engage.

Quando si compila un modulo web o si visita una pagina di destinazione ospitata dal Marketo Engage, per impostazione predefinita le informazioni vengono inviate tramite un protocollo non sicuro (HTTP). In base alla politica aziendale, potrebbe essere utile proteggere le informazioni inviate a Marketo tramite (HTTPS). Ad esempio, quando visiti `http://info.mydomain.com/`, adesso sarà `https://info.mydomain.com/`.

Per impostazione predefinita, il Marketo Engage tiene traccia di &quot;Visited Web Page&quot; e &quot;Click Link on Web Page&quot; su un protocollo HTTP non sicuro. Se desideri proteggere i collegamenti di tracciamento con il proprio certificato, è necessario che Marketo crei un server non condiviso separato per abilitarlo. Proteggere tutti gli aspetti dell’interazione di un contatto con te in genere significa proteggere sia le pagine di destinazione che i collegamenti di tracciamento.

Alla fine del 2022 sono state apportate modifiche alla modalità di protezione dei domini di collegamento delle pagine di destinazione e di tracciamento. [Ulteriori informazioni](https://nation.marketo.com/t5/product-blogs/changes-to-marketo-engage-secured-domains-platform/ba-p/329305){target="_blank"}.

Se desideri utilizzare SSL per le pagine di destinazione del Marketo Engage, contatta il team dell’account Adobe (il tuo account manager).
