---
solution: Marketo Engage
product: marketo
title: Assassino spam
description: INSERISCI QUI IL TESTO
level: Beginner, Intermediate
feature: Email Editor
hide: true
hidefromtoc: true
source-git-commit: 0157bc64444151a43bf464158d508e84d75b3427
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 3%

---

# Assassino spam {#spam-assassin}

Utilizzando SpamAssassin in Marketo Engage, puoi testare il contenuto delle e-mail e vedere la probabilità che gli ISP o i provider di cassette postali le contrassegnino come spam.

SpamAssassin analizza il contenuto e assegna un punteggio in base a vari criteri. Minore è il punteggio, meglio è. È importante mantenere un punteggio basso, in quanto l’invio di e-mail con un punteggio elevato può influire negativamente sul recapito messaggi complessivo.

## Accedere al rapporto Spam {#access-the-spam-report}

1. Dalla schermata Simula, fai clic sul pulsante **Rapporto spam**.

SCHERMATA

1. Viene generato un rapporto di posta indesiderata.

SCHERMATA

1. Controlla i punteggi e le descrizioni di ogni elemento.

>[!IMPORTANT]
>
>Se il punteggio complessivo è superiore a 5, l’e-mail potrebbe essere bloccata o contrassegnata come spam al momento della consegna.

1. Se ritieni che il punteggio sia troppo alto, modifica il contenuto nel Designer e-mail, quindi esegui nuovamente il rapporto Spam fino a quando il punteggio non si trova dove desideri che sia.

SCHERMATA

>[!NOTE]
>
>Il punteggio spam viene derivato tramite SpamAssassin e le regole non sono di proprietà di Adobe. Ulteriori dettagli su queste regole sono disponibili nella [documentazione di SpamAssassin](https://spamassassin.apache.org/#_blank). Un elenco completo degli errori [è disponibile qui](https://spamassassin.apache.org/old/tests_3_0_x.html?utm_source=chatgpt.com).
