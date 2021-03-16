---
unique-page-id: 11380774
description: Punteggio account - Documenti Marketo - Documentazione del prodotto
title: Punteggio account
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Punteggio account {#account-score}

Il punteggio dell&#39;account è una parte fondamentale della gestione dell&#39;account Target. Consente di determinare il livello di coinvolgimento degli account.

## Cos’è il punteggio dell’account? {#what-is-account-scoring}

È un approccio sistematico progettato per aiutare i team di vendita e marketing a identificare e dare priorità alle aziende (incluse le prospettive) che hanno più probabilità di fare un acquisto.

Nel complesso mondo dei processi di acquisto B2B, è raro che un singolo individuo prenda una decisione di acquisto. Ci sono spesso diversi ruoli coinvolti, ciascuno con le proprie esigenze. Il punteggio basato su account tiene conto di questo aspetto aggregando i punteggi dei lead da più lead e fornendo un punteggio a livello di account.

## Esempi comuni {#common-examples}

<table> 
 <tbody>
  <tr>
   <td><strong>Punteggio di coinvolgimento dell’account</strong></td> 
   <td>Profondità di coinvolgimento in base alle attività comportamentali tracciate tra vari canali (ad esempio e-mail, web e annunci) da persone in account target specifici.</td>
  </tr>
  <tr>
   <td><strong>Punteggio di interesse del prodotto dell'account</strong></td>
   <td>Persone di account target che mostrano interesse per i contenuti di un prodotto specifico (ad esempio download di un white paper).</td> 
  </tr>
  <tr>
   <td><strong>Punteggio di coinvolgimento Web dell'account</strong></td>
   <td>Persone da account di destinazione che visitano il canale web. Puoi creare lo stesso punteggio per misurare il coinvolgimento del canale da e-mail, annunci pubblicitari o altri canali.</td> 
  </tr>
 </tbody>
</table>

## Come configurare il punteggio account {#how-to-configure-account-score}

>[!NOTE]
>
>Per calcolare i punteggi del conto, devi innanzitutto creare i punteggi dei lead. Marketo TAM aggrega automaticamente i punteggi dei lead ai punteggi dei conti. Ad esempio, prenderemo due degli esempi precedenti (_Punteggio di interesse del prodotto dell&#39;account_ e _Punteggio di coinvolgimento del web dell&#39;account_).
>
>Innanzitutto, crea campi per il punteggio lead che acquisiscono i dettagli rilevanti da ciascun lead di un account target.\
>Quindi assegna i punteggi lead ai rispettivi punteggi del conto:\
>Punteggio di interesse del prodotto dell’account = SOMMA (Punteggio di interesse del prodotto principale)\
>Punteggio di coinvolgimento Web dell&#39;account = SUM (Punteggio di coinvolgimento Web principale)

>[!NOTE]
>
>Gli utenti possono creare più punteggi di coinvolgimento dell’account e assegnare diversi punteggi di persona a diversi punteggi di account.

Una volta configurato il punteggio lead, procedi seguendo i passaggi seguenti.

1. Fai clic su **Amministratore**.

   ![](assets/one-1.png)

1. Fai clic su **Gestione account di destinazione**.

   ![](assets/account-score-2.png)

1. In Campi di valutazione, fai clic su **Modifica**.

   ![](assets/account-score-3.png)

   >[!NOTE]
   >
   >Puoi scegliere fino a **cinque** campi per calcolare il punteggio dell&#39;account.

1. Inserisci il nome del punteggio account, fai clic sul menu a discesa **Seleziona punteggio persona** e seleziona il punteggio corrispondente.

   ![](assets/four.png)

1. Fai clic su **+Aggiungi** per aggiungere altri punteggi.

   ![](assets/five.png)

1. Aggiungi tutti i punteggi desiderati. Al termine, fai clic su **Salva**.

   ![](assets/six.png)
