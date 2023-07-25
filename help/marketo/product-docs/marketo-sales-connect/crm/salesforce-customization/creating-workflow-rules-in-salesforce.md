---
unique-page-id: 14745823
description: Creazione di regole del flusso di lavoro in Salesforce - Documenti Marketo - Documentazione del prodotto
title: Creazione di regole del flusso di lavoro in Salesforce
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Creazione di regole del flusso di lavoro in Salesforce {#creating-workflow-rules-in-salesforce}

Quando si utilizzano in parallelo Marketo Sales Insight (MSI) e Marketo Sales Connect (MSC), la funzione MSI Best Bets in Salesforce non viene aggiornata. Tutte le altre funzioni MSI funzionano normalmente (visualizzazione di momenti interessanti nell’iFrame, invio di e-mail, aggiunta a campagne, ecc.). Questo articolo offre una soluzione alternativa per far funzionare di nuovo gli elementi di maggiore rilevanza.

>[!NOTE]
>
>Questo interessa solo i clienti che utilizzano **entrambi** MSI e MSE e che desiderano utilizzare la funzione Elementi di maggiore rilevanza in MSI. Se non hai bisogno/utilizza gli elementi di maggiore rilevanza, puoi ignorarli.

## Guida introduttiva {#getting-started}

La soluzione alternativa include la creazione di nuove regole del flusso di lavoro per copiare i valori dai nuovi campi MSE nei vecchi campi MSI. È necessario creare quattro regole di flusso di lavoro per l&#39;oggetto Contact e le stesse quattro regole di flusso di lavoro per l&#39;oggetto Lead nella propria istanza Salesforce. Potrebbe essere necessario disporre dei diritti di amministratore CRM (a seconda del ruolo e della configurazione in CRM).

Di seguito sono riportati i nomi consigliati delle regole del flusso di lavoro e le relative descrizioni. Questi sono applicabili all&#39;oggetto Contact e Lead:

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>Aggiorna campo descrizione momento di interesse</td> 
   <td><p>Copia da: ultima descrizione di Marketo Engagement<br>Copia in: Descrizione ultimo momento di interesse</p></td> 
  </tr> 
  <tr> 
   <td>Aggiorna il campo del tipo di momento di interesse</td> 
   <td><p>Copia da: ultimo tipo di coinvolgimento Marketo<br>Copia in: Ultimo tipo di momento di interesse</p></td> 
  </tr> 
  <tr> 
   <td>Aggiorna il campo Origine momento di interesse</td> 
   <td><p>Copia da: ultima origine di Marketo Engagement<br>Copia in: Origine ultimo momento di interesse</p></td> 
  </tr> 
  <tr> 
   <td>Aggiorna il campo Data momento di interesse</td> 
   <td><p>Copia da: data ultimo coinvolgimento Marketo<br>Copia in: data ultimo momento di interesse</p></td> 
  </tr> 
 </tbody> 
</table>

## Istruzioni {#instructions}

1. Dopo aver fatto clic su **Configurazione**, cerca **Flusso di lavoro** e seleziona **Regole flusso di lavoro**.

   ![](assets/one-1.png)

1. Seleziona **Nuova regola**.

   ![](assets/two-1.png)

1. Fai clic sull’elenco a discesa Oggetto e seleziona **Lead**, quindi fai clic su **Successivo**.

   ![](assets/three-1.png)

1. Immetti &quot;Aggiorna campo descrizione momento di interesse&quot; come nome della regola. Seleziona il pulsante di opzione **e ogni volta che viene modificato**. Nel menu a discesa Criteri regola, seleziona **formula restituisce true**. Cercare e selezionare la funzione ISCHANGED. Quindi, evidenzia il valore del campo predefinito e fai clic su **Inserisci campo**.

   ![](assets/four-1.png)

1. Nella finestra a comparsa &quot;Inserisci campo&quot;, scegliere **Descrizione ultimo coinvolgimento Marketo** e fai clic su **Inserisci**.

   ![](assets/five-1.png)

1. Clic **Salva e Successivo**.

   ![](assets/6.png)

1. Nel menu a discesa Aggiungi azione flusso di lavoro, seleziona **Nuovo aggiornamento campo**.

   ![](assets/seven.png)

1. Nel campo Nome, immetti &quot;Aggiorna campo descrizione momento di interesse&quot; (viene generato automaticamente un nome univoco). Nel menu a discesa Campo da aggiornare, scegli **Descrizione ultimo momento di interesse**. Seleziona la **Utilizzare una formula per impostare un nuovo valore** , quindi fare clic su **Mostra editor formule**.

   ![](assets/eight.png)

1. Fai clic su **Inserisci campo** pulsante.

   ![](assets/9a.png)

1. Seleziona **Descrizione ultimo coinvolgimento Marketo** e fai clic su **Inserisci**. Nella pagina successiva fare clic su **Salva**.

   ![](assets/nine.png)

1. Clic **Fine**.

   ![](assets/twelve.png)

1. Clic **Attiva** per attivare la regola del flusso di lavoro.

   ![](assets/thirteen.png)

   Dopo l&#39;ultimo passaggio, è possibile scegliere di clonare la regola del flusso di lavoro per gli altri campi elencati nella sezione Guida introduttiva: Desc, Type, Source, Date. Dopo aver completato le quattro regole del flusso di lavoro nell&#39;oggetto Contact, ripetere le stesse operazioni per l&#39;oggetto Lead.
