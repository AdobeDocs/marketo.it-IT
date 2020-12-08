---
unique-page-id: 11380774
description: Valutazione account - Documenti Marketo - Documentazione prodotto
title: Punteggio account
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# Punteggio account {#account-score}

Il punteggio account è una parte fondamentale del marketing basato su account. Consente di determinare il livello di coinvolgimento degli account.

## Cos&#39;è il punteggio account? {#what-is-account-scoring}

È un approccio sistematico progettato per aiutare i team di vendita e marketing a identificare e assegnare priorità alle aziende (inclusi i potenziali clienti) che più probabilmente effettueranno un acquisto.

Nel complesso mondo dei processi di acquisto B2B, è raro che un singolo individuo prenda una decisione di acquisto. Ci sono spesso diversi ruoli coinvolti, ciascuno con le proprie esigenze. Il punteggio basato su account tiene conto di questo fattore aggregando i punteggi dei lead da più lead e fornendo un punteggio a livello di conto.

## Esempi comuni {#common-examples}

| **Punteggio di coinvolgimento account** | Profondità di coinvolgimento in base alle attività comportamentali tracciate tra i vari canali (ad es. e-mail, web e annunci) da persone in specifici account target. |
|---|---|
| **Punteggio interessi prodotto account** | Persone provenienti da account di destinazione che mostrano interesse per il contenuto di un prodotto specifico (ad esempio, scaricare un white paper). |
| **Punteggio coinvolgimento Web account** | Persone dagli account di destinazione che visitano il canale Web. Lo stesso punteggio può essere creato per misurare il coinvolgimento dei canali tramite e-mail, annunci pubblicitari o altri canali. |

## Come configurare il punteggio account {#how-to-configure-account-score}

>[!NOTE]
>
>**Spiegazione**
>
>Per calcolare i punteggi dei conti, è innanzitutto necessario creare i punteggi dei lead. Marketo ABM aggrega automaticamente i punteggi dei lead ai punteggi dei conti. Ad esempio, prenderemo due degli esempi di cui sopra (*Account *Punteggio interessi *prodotto* e punteggio *di coinvolgimento Web account*).
>
>Innanzitutto, create campi per il punteggio iniziale che acquisiscano i dettagli rilevanti da ciascun lead di un account di destinazione.\
>Quindi assegnate i punteggi dei lead ai rispettivi punteggi del conto:\
>Punteggio interessi prodotto account = SUM (Punteggio interessi prodotto lead)\
>Punteggio coinvolgimento Web account = SUM (Punteggio coinvolgimento Web principale)

>[!NOTE]
>
>Gli utenti possono creare più punteggi di coinvolgimento dell&#39;account e assegnare diversi punteggi di persona a diversi punteggi di account.

Una volta configurato il punteggio iniziale, procedete come segue.

1. Fate clic su **Admin**.

   ![](assets/one-1.png)

1. Fate clic su **ABM**.

   ![](assets/two-1.png)

1. In Campi punteggio, fare clic su **Modifica**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >È possibile scegliere fino a **cinque campi **per calcolare il punteggio account.

1. Immettete il nome Valutazione account, fate clic sul menu a discesa **Seleziona punteggio** persona e selezionate la valutazione corrispondente.

   ![](assets/four.png)

1. Fare clic su **+Aggiungi **per aggiungere altri punteggi.

   ![](assets/five.png)

1. Aggiungete tutti i punteggi desiderati. Al termine, fate clic su **Salva** .

   ![](assets/six.png)

