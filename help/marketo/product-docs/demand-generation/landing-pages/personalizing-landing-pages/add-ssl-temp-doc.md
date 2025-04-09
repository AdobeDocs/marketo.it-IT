---
description: Aggiungere SSL alle pagine di destinazione - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere SSL alle pagine di destinazione
hide: true
hidefromtoc: true
feature: Landing Pages
exl-id: 00ec2d91-3d4f-4671-af9d-9750c1642d40
source-git-commit: 1112af01c08835876f4a2385f304a33e2ddd48ff
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Aggiungere SSL alle pagine di destinazione {#add-ssl-to-your-landing-pages}

La crittografia SSL (Secure Socket Layer) consente di rendere sicure tutte le pagine di destinazione di un’istanza di Marketo Engage.

Quando si compila un modulo web o si visita una pagina di destinazione ospitata da Marketo Engage, per impostazione predefinita le informazioni vengono inviate tramite un protocollo non sicuro (HTTP). In base alla politica aziendale, potrebbe essere utile proteggere le informazioni inviate a Marketo tramite (HTTPS). Ad esempio, quando visiti `http://info.mydomain.com/`, adesso sarà `https://info.mydomain.com/`.

Marketo Engage tiene traccia di &quot;Visited Web Page&quot; e &quot;Click Link on Web Page&quot; per impostazione predefinita su un protocollo HTTP non sicuro. Se desideri proteggere i collegamenti di tracciamento con il proprio certificato, è necessario che Marketo crei un server non condiviso separato per abilitarlo. Proteggere tutti gli aspetti dell’interazione di un contatto con te in genere significa proteggere sia le pagine di destinazione che i collegamenti di tracciamento.

SCHERMATA

## Abilita certificazione SSL {#enable-ssl-certification}

Aggiungi automaticamente SSL per tutti gli alias di dominio creati come parte delle regole della pagina di destinazione.

1. Vai all&#39;area **Amministratore**.

   SCHERMATA

1. Seleziona **Pagine di destinazione** dalla struttura. Nella scheda **Regole**, fai clic sull&#39;elenco a discesa **Nuovo** e seleziona **Nuovo alias di dominio**.

   SCHERMATA

1. Selezionare la casella di controllo **Genera certificato SSL**.

   SCHERMATA

Questo aggiunge automaticamente un certificato SSL per questo dominio.

SCHERMATA

## Abilita SSL per il dominio predefinito {#enable-ssl-default-domain}

SCHERMATA

>[!NOTE]
>
>* La colonna Certificato SSL nell’elenco mostra lo stato del certificato per tutti gli alias di dominio creati dopo il rilascio di questa funzione (DATE). Se SSL era abilitato per un dominio tramite il supporto Marketo, il certificato continuerà a esistere ma non verrà visualizzato nella tabella. Questa tabella riflette solo i certificati SSL per i domini aggiunti utilizzando i passaggi descritti in questo articolo.
>
>* Possono essere necessari fino a tre minuti perché SSL sia nello stato READY. È necessario aggiornare la pagina per visualizzare le modifiche.
