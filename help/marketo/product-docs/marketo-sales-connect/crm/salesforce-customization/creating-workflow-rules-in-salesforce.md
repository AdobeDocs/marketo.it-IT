---
unique-page-id: 14745823
description: Creazione di regole di workflow in Salesforce - Documenti Marketo - Documentazione prodotto
title: Creazione di regole per il flusso di lavoro in Salesforce
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# Creazione di regole per il flusso di lavoro in Salesforce {#creating-workflow-rules-in-salesforce}

Quando si utilizzano parallelamente Marketo Sales Insight (MSI) e Marketo Sales Connect (MSC), la funzione MSI Best Bets in Salesforce non verrà aggiornata. Tutte le altre funzioni MSI funzionano normalmente (visualizzazione di momenti interessanti nell’iFrame, invio di e-mail, aggiunta a campagne, ecc.). Questo articolo offre una soluzione alternativa per far funzionare di nuovo Best Bets.

>[!NOTE]
>
>Questo interessa solo i clienti che utilizzano **sia** MSI che MSE e che desiderano utilizzare la funzione Best Bets in MSI. Se non avete bisogno/utilizzate le Scommesse migliori, potete ignorarlo.

## Guida introduttiva {#getting-started}

La soluzione alternativa include la creazione di nuove regole di flusso di lavoro per copiare i valori dai nuovi campi MSE nei vecchi campi MSI. Dovrai creare quattro regole di flusso di lavoro per l&#39;oggetto Contatto e le stesse quattro regole di flusso di lavoro per l&#39;oggetto Lead nella tua istanza Salesforce. Questo potrebbe richiedere l&#39;utilizzo dei diritti di amministratore CRM (a seconda del ruolo e della configurazione in CRM).

Di seguito sono riportati i nomi consigliati delle regole del flusso di lavoro e la descrizione di ciascuna di esse. Si applicano all’oggetto Contatto e Lead:

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>Aggiorna Campo Desc Momento Interessante</td> 
   <td><p>Copia da: Desc. ultimo coinvolgimento Marketo<br>Copia in: Ultimo interessante momento</p></td> 
  </tr> 
  <tr> 
   <td>Aggiorna campo Interessante tipo di momento</td> 
   <td><p>Copia da: Ultimo tipo di coinvolgimento del marketing<br>Copia in: Ultimo tipo di momento interessante</p></td> 
  </tr> 
  <tr> 
   <td>Aggiorna campo Interessante origine momento</td> 
   <td><p>Copia da: Ultima origine di coinvolgimento Marketo<br>Copia in: Ultima origine momento interessante</p></td> 
  </tr> 
  <tr> 
   <td>Aggiorna campo data momento interessante</td> 
   <td><p>Copia da: Data ultimo coinvolgimento Marketo<br>Copia in: Data ultimo momento interessante</p></td> 
  </tr> 
 </tbody> 
</table>

## Istruzioni {#instructions}

1. Dopo aver fatto clic su **Setup**, cercare **Workflow** e selezionare **Workflow Rules**.

   ![](assets/one-1.png)

1. Selezionare **Nuova regola**.

   ![](assets/two-1.png)

1. Fare clic sul menu a discesa Oggetto e selezionare **Lead**, quindi fare clic su **Avanti**.

   ![](assets/three-1.png)

1. Immettete &quot;Update Interesting Moment Desc Field&quot; come nome della regola. Selezionare il pulsante di scelta **creato e ogni volta che viene modificato**. Nel menu a discesa Criteri regola, selezionare **formula restituisce true**. Cercare e selezionare la funzione ISCHANGED. Evidenziare quindi il valore del campo predefinito e fare clic su **Inserisci campo**.

   ![](assets/four-1.png)

1. Nella finestra a comparsa &quot;Inserisci campo&quot;, scegliere **Ultimo punto di coinvolgimento del marketing** e fare clic su **Inserisci**.

   ![](assets/five-1.png)

1. Fare clic su **Save &amp; Next**.

   ![](assets/6.png)

1. Nel menu a discesa Aggiungi azione flusso di lavoro, selezionare **Nuovo aggiornamento campo**.

   ![](assets/seven.png)

1. Nel campo Nome, immettete &quot;Update Interesting Moment Desc Field&quot; (Aggiorna campo Moment Desc Interessante) (il nome univoco verrà generato automaticamente). Nel menu a discesa Campo da aggiornare, scegliete **Ultima descrizione momento interessante**. Selezionare il pulsante di scelta **Utilizzare una formula per impostare un nuovo valore**, quindi fare clic su **Mostra editor formule**.

   ![](assets/eight.png)

1. Fare clic sul pulsante **Inserisci campo**.

   ![](assets/9a.png)

1. Selezionare **Desc. ultimo coinvolgimento del marketing**, quindi fare clic su **Inserisci**. Nella pagina successiva, fare clic su **Salva**.

   ![](assets/nine.png)

1. Fare clic su **Fine**.

   ![](assets/twelve.png)

1. Fare clic su **Attiva** per attivare la regola del flusso di lavoro.

   ![](assets/thirteen.png)

   Dopo l’ultimo passaggio, potete scegliere di duplicare la regola del flusso di lavoro per gli altri campi elencati nella sezione Guida introduttiva: Descrizione, Tipo, Origine, Data. Dopo aver completato le quattro regole del flusso di lavoro nell&#39;oggetto Contatto, ripetere lo stesso per l&#39;oggetto Lead.
