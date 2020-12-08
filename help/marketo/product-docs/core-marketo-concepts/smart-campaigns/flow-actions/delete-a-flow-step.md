---
unique-page-id: 1146987
description: Eliminazione di un passaggio di flusso - Documenti Marketo - Documentazione prodotto
title: Eliminare un passaggio di flusso
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# Eliminare un passaggio di flusso {#delete-a-flow-step}

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

>[!CAUTION]
>
>La rimozione dei passaggi di flusso, *in particolare dei passaggi* di attesa dalle campagne smart attive, può produrre risultati imprevisti. **Leggete attentamente questo articolo.**

Prima facciamo le basi. Ecco come rimuovere un passaggio di flusso indesiderato da una campagna intelligente. 1. In Flusso campagna intelligente, fai clic sull’icona X per eliminare qualsiasi passaggio di flusso.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Fate clic su **Elimina**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Semplice e facile, giusto? Beh, la maggior parte del tempo...

   >[!CAUTION]
   >
   >L’eliminazione, l’aggiunta e lo spostamento dei passaggi all’interno di una campagna **attiva** possono dare risultati imprevisti. Prendete in considerazione la creazione di una nuova campagna, il test e quindi il passaggio a un&#39;altra.

   Le modifiche possono essere apportate a una campagna attiva, ma possono avere conseguenze impreviste. Di seguito sono riportati i dettagli:

   **Campagne intelligenti in batch**

   Se la campagna:

   1. **Mai corso.** Apportate tutte le modifiche desiderate. Non colpirà nessuno fino a quando non esegui quella campagna.
   1. **È una campagna intelligente ricorrente.** Le modifiche interesseranno le persone nelle esecuzioni future, non le esecuzioni precedenti.
   1. **È già stato eseguito senza passaggi di attesa.** Nessun utente sarà interessato perché la campagna è inattiva dopo l&#39;esecuzione.
   1. **Sta correndo in questo momento.** Le modifiche possono causare un comportamento imprevisto in base alla temporizzazione e ai dettagli dell&#39;eliminazione. È consigliabile NON modificare una campagna batch in esecuzione. Per i casi di emergenza, scopri come [interrompere una campagna](../../../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md)intelligente in corso.

   1. **Sono già stati eseguiti con passi di attesa.** Diversi dettagli su questo.\
      Quando una persona entra in un passaggio di attesa, scende la durata e a quale PASSAGGIO NUMERO tornare. Vedere l&#39;esempio seguente.

   **Attiva campagne intelligenti**

   1. **Nessun passaggio di attesa.** Se elimini un passaggio normale, verranno interessati solo gli utenti che in futuro avranno eseguito la campagna.
   1. **Con i passi di attesa.** Per le campagne batch, vedere l&#39;esempio seguente. Si applica la stessa logica.

   >[!NOTE]
   >
   >**Esempio**
   >
   >    
   >    
   >1. Una campagna intelligente ha 3 passaggi.
   >
   >   * PASSAGGIO 1. Invia e-mail n. 1
   >   * PASSAGGIO 2. Aspetta 1 settimana
   >   * PASSAGGIO 3. Invia e-mail #2
   >
   >1. Le persone che hanno colpito il **passo 2** aspetteranno 1 settimana prima di passare al **passo 3**.
   >1. Si elimina il **Passaggio 2** durante la settimana.
   >1. La gente continuerà ad aspettare una settimana. (non tornano automaticamente nel flusso).
   >1. Quando finalmente torneranno, cercheranno di andare al **Passo 3**. Loro non la troveranno.
   >1. **IMPORTANTE:** Poiché ora ci sono solo 2 passi, le *persone non riceveranno e-mail #2.*


Modifiche a una campagna attiva

Scopri questa funzione e potrai realizzare campagne intelligenti. Wow!
