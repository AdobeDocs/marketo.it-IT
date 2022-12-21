---
unique-page-id: 1146987
description: Eliminare un passaggio del flusso - Documentazione di Marketo - Documentazione del prodotto
title: Eliminare un passaggio del flusso
exl-id: 039a1e80-48cc-47f9-9e1a-459f89bf0730
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Eliminare un passaggio del flusso {#delete-a-flow-step}

>[!CAUTION]
>
>Rimozione dei passaggi del flusso _particolarmente attendi_ da campagne avanzate attive, possono verificarsi risultati imprevisti. **Leggete attentamente questo articolo.**

Prima facciamo le nozioni di base. Ecco come rimuovere un passaggio di flusso indesiderato da una campagna intelligente. 1. Nel flusso della campagna intelligente, fai clic sull’icona X per eliminare qualsiasi passaggio di flusso.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Fai clic su **Elimina**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Semplice e facile, vero? Beh, la maggior parte delle volte...

   >[!CAUTION]
   >
   >Eliminazione, aggiunta e spostamento di passaggi all&#39;interno di un **attivo** Campaign può sicuramente avere risultati imprevisti. Prendi in considerazione la creazione di una nuova campagna, il test e quindi il passaggio.

   I cambiamenti possono essere apportati a una campagna attiva ma possono avere conseguenze impreviste. Di seguito sono riportati i dettagli:

   **Campagne avanzate in batch**

   Se la campagna:

   1. **Mai corso.** Apporta tutte le modifiche desiderate. Non influenzerà nessuno finché non esegui quella campagna.
   1. **È una campagna intelligente ricorrente.** Le modifiche avranno effetto sulle persone nelle esecuzioni future, non sulle esecuzioni precedenti.
   1. **È già stato eseguito senza passaggi di attesa.** Non ci saranno persone interessate perché la campagna è inattiva dopo l&#39;esecuzione.
   1. **Sta correndo in questo momento.** Le modifiche possono causare un comportamento imprevisto a seconda della data e dei dettagli dell’eliminazione. È consigliabile NON modificare una campagna batch attiva in esecuzione. Per i casi di emergenza, scopri come [interrompe una campagna intelligente in esecuzione](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md).

   1. **Sono già stati eseguiti con passaggi di attesa.** Diversi dettagli su questo.\
      Quando una persona entra in un passaggio di attesa, scende la durata e a quale PASSAGGIO NUMERO tornare. Vedi l&#39;esempio seguente.

   **Attivazione di campagne avanzate**

   1. **Nessun passaggio di attesa.** Se elimini un passaggio normale, verranno interessate solo le persone che in futuro avranno eseguito la campagna.
   1. **Con passaggi di attesa.** Vedi l&#39;esempio seguente per le campagne batch. Si applica la stessa logica.

   >[!NOTE]
   >
   >**Esempio**
   >
   >1. Una campagna intelligente ha 3 passaggi.
      >    * PASSAGGIO 1. Invia e-mail n. 1
      >    * PASSAGGIO 2. Attendi 1 settimana
      >    * PASSAGGIO 3. Invia e-mail n. 2
   >
   >1. Persone che hanno colpito **Passaggio 2** attenderà una settimana prima di passare a **Passaggio 3**.
   >1. Elimina **Passaggio 2** durante la settimana.
   >1. La gente continuerà ad aspettare la 1 settimana. (non tornano automaticamente nel flusso.)
   >1. Quando alla fine torneranno, cercheranno di andare a **Passaggio 3**. Loro non la troveranno.
   >1. **IMPORTANTE:** Poiché ora sono presenti solo 2 passaggi, il *le persone non riceveranno e-mail n. 2.*


Apportare modifiche a una campagna attiva

Comprendi questa funzione e sarai in grado di gestire le campagne intelligenti.
