---
description: Aggiungere SSL alle pagine di destinazione - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere SSL alle pagine di destinazione
hide: true
hidefromtoc: true
feature: Landing Pages
source-git-commit: 0e73866a4187d7bff67ce199e8d01e55081bcbef
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Aggiungere SSL alle pagine di destinazione {#add-ssl-to-your-landing-pages}

Scopri come aggiungere l’alias del dominio del tuo marchio (ad esempio, `http://business.adobe.com`) alle pagine di destinazione create in Marketo Engage in modo che sia possibile accedervi nell’ambito dei domini del tuo marchio.

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

## Abilita SSL per il dominio predefinito

SCHERMATA

>[!NOTE]
>
>* La colonna Certificato SSL nell’elenco mostra lo stato del certificato per tutti gli alias di dominio creati dopo il rilascio di questa funzione (DATE). Se SSL era abilitato per un dominio tramite il supporto Marketo, il certificato continuerà a esistere ma non verrà visualizzato nella tabella. Questa tabella riflette solo i certificati SSL per i domini aggiunti utilizzando i passaggi descritti in questo articolo.
>
>* Possono essere necessari fino a tre minuti perché SSL sia nello stato READY. È necessario aggiornare la pagina per visualizzare le modifiche.
