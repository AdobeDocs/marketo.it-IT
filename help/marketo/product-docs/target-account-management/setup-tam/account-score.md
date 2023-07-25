---
unique-page-id: 11380774
description: Punteggio account - Documentazione di Marketo - Documentazione del prodotto
title: Punteggio account
exl-id: 68fb5f41-f715-4a4d-b4da-9db4dc38d67d
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Punteggio account {#account-score}

Il punteggio dell’account è una parte vitale della gestione dell’account Target. Consente di determinare il livello di coinvolgimento degli account.

## Cos’è il punteggio dell’account? {#what-is-account-scoring}

Si tratta di un approccio sistematico progettato per aiutare i team di vendita e marketing a identificare e assegnare le priorità alle aziende (inclusi i potenziali clienti) che hanno più probabilità di effettuare un acquisto.

Nel complesso mondo dei processi di acquisto B2B, è raro che un singolo individuo prenda una decisione di acquisto. Spesso sono coinvolti diversi ruoli, ciascuno con le proprie esigenze. Il punteggio basato sull’account ne tiene conto aggregando i punteggi dei lead da più lead e fornendo un punteggio a livello di account.

## Esempi comuni {#common-examples}

<table> 
 <tbody>
  <tr>
   <td><strong>Punteggio di coinvolgimento dell’account</strong></td> 
   <td>Profondità di coinvolgimento basata sulle attività comportamentali tracciate tra vari canali (ad esempio e-mail, web, annunci) da persone in account di destinazione specifici.</td>
  </tr>
  <tr>
   <td><strong>Punteggio interesse prodotto account</strong></td>
   <td>Persone da account target che mostrano interesse per il contenuto da un prodotto specifico (ad esempio, il download di un white paper).</td> 
  </tr>
  <tr>
   <td><strong>Punteggio di coinvolgimento web dell’account</strong></td>
   <td>Persone dagli account di destinazione che visitano il canale web. È possibile creare lo stesso punteggio per misurare il coinvolgimento dei canali da e-mail, annunci pubblicitari o altri canali.</td> 
  </tr>
 </tbody>
</table>

## Come configurare il punteggio dell’account {#how-to-configure-account-score}

>[!NOTE]
>
>Per calcolare i punteggi dei conti, devi innanzitutto creare i punteggi dei lead. Marketo TAM aggrega automaticamente i punteggi dei lead per i punteggi degli account. Ad esempio, prendiamo due degli esempi precedenti (_Punteggio interesse prodotto account_ e _Punteggio di coinvolgimento web dell’account_).
>
>Innanzitutto, crea dei campi di valutazione del lead che acquisiscono dettagli rilevanti da ciascun lead di un account target.\
>Quindi assegna i punteggi dei lead ai rispettivi punteggi dell’account:\
>Punteggio interesse prodotto conto = SOMMA (Punteggio interesse prodotto lead)\
>Punteggio coinvolgimento Web account = SUM (punteggio coinvolgimento Web lead)

>[!NOTE]
>
>Gli utenti possono creare più punteggi di coinvolgimento dell’account e assegnare punteggi di persona diversi a punteggi di account diversi.

Dopo aver configurato il punteggio del lead, procedi seguendo i passaggi seguenti.

1. Clic **Amministratore**.

   ![](assets/one-1.png)

1. Clic **Gestione account di destinazione**.

   ![](assets/account-score-2.png)

1. In Campi punteggio, fai clic su **Modifica**.

   ![](assets/account-score-3.png)

   >[!NOTE]
   >
   >Puoi scegliere fino a **cinque** campi per calcolare il Punteggio conto.

1. Inserisci il nome del Punteggio account, fai clic su **Seleziona punteggio persona** e selezionare il punteggio corrispondente.

   ![](assets/four.png)

1. Clic **+Aggiungi** per aggiungere altri punteggi.

   ![](assets/five.png)

1. Aggiungi tutti i punteggi desiderati. Clic **Salva** al termine.

   ![](assets/six.png)
