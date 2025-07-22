---
description: Eseguire una campagna - Documentazione di Marketo - Documentazione del prodotto
title: Esegui campagna
exl-id: d550cf08-b295-4289-9bb0-79d81cabc245
feature: Smart Campaigns
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# Esegui campagna {#execute-campaign}

Una campagna eseguibile, come altre campagne, contiene un elenco avanzato, un flusso e una pianificazione. A differenza di altre campagne, non puoi pianificarle o attivarle. Può essere richiamato solo da un’altra campagna tramite il passaggio di flusso Esegui campagna. I passaggi di flusso nella campagna eseguibile vengono eseguiti in serie con la campagna principale (a differenza di Campagna richieste, che viene eseguita in parallelo in una campagna con trigger separata).

>[!NOTE]
>
>Le campagne eseguibili sono sempre figli della campagna (principale) che le chiama.

## Quando utilizzare Esegui campagna {#when-to-use-execute-campaign}

Ci sono molte cose che puoi fare con una campagna eseguibile. Sono progettate per facilitare attività operative comuni, come il routing dei lead, la gestione del ciclo di vita e il punteggio (tra gli altri) e possono essere utilizzate per eseguire lo stesso flusso di lavoro dall’interno di campagne batch o attivate.

Puoi utilizzarli anche quando devi eseguire un flusso separato, ma devi dipendere dai risultati di tale flusso nelle scelte dei passaggi successivi del flusso (ad esempio, in questo caso, fai così).

Esegui campagna è un miglioramento rispetto a [Richiedi campagna](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/request-campaign.md), in quanto può essere eseguita in serie, mentre quest&#39;ultima viene eseguita solo in parallelo.

>[!NOTE]
>
>Wait Steps e Webhook non saranno mai compatibili con le campagne eseguibili. Per questi, dovrai utilizzare Richiedi campagna.

## Come creare una campagna eseguibile {#how-to-create-an-executable-campaign}

1. Fare clic con il pulsante destro del mouse sul programma desiderato e selezionare **[!UICONTROL New Smart Campaign]**.

   ![](assets/execute-campaign-1.png)

1. Assegnare un nome, selezionare la casella di controllo **[!UICONTROL Executable]** e fare clic su **[!UICONTROL Create]**.

   ![](assets/execute-campaign-2.png)

1. Definisci l’elenco avanzato e il flusso, come per qualsiasi altra campagna avanzata.

Puoi anche clonare una campagna avanzata esistente. Se si clona una campagna eseguibile esistente, sarà comunque necessario selezionare la casella di controllo **[!UICONTROL Executable]** dopo averla denominata.

>[!NOTE]
>
>Non puoi clonare una campagna che contiene trigger.

## Usa contesto token campagna principale {#use-parent-campaign-token-context}

Se è impostato su true, i seguenti contesti di token vengono inviati nella campagna figlio (quella in esecuzione):

* I miei token
* Token campagna
* Token programma
* Token membro
* [Token di attivazione](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) (se chiamato da una campagna attivata)

**Interazione API**

Quando si utilizza Schedule o Request Campaign [ nell&#39;API](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/assets/smart-campaigns#batch), entrambi consentono di trasmettere valori per I miei token, che sostituiscono i valori impostati per tali token nella campagna che si sta chiamando. Se tale campagna esegue un’altra campagna e imposta &quot;Use Parent Context&quot; (Usa contesto padre) su True, utilizzerà i valori trasmessi tramite l’API, anziché i valori impostati nell’applicazione.

## Aspetti da considerare {#things-to-note}

* L’elenco avanzato escluderà chiunque non sia idoneo. Se una persona risulta idonea, il record di attività Campagna eseguita risultante le elencherà come &quot;Qualificate: TRUE&quot; (e FALSE in caso contrario)
* Si applicano le regole di qualificazione della pianificazione della campagna (Impostazioni campagna avanzata nella scheda Pianificazione)
* Impossibile chiamare le campagne eseguibili in più aree di lavoro
* Se si utilizza l&#39;azione di flusso [Rimuovi dal flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) destinata a una campagna eseguibile, verrà eseguita sia la campagna figlio che la campagna padre
* Sfruttare l’ereditarietà dei token: ad esempio, se disponi di un singolo flusso di punteggio comune attivato da più risorse diverse, puoi definire un punteggio My Token predefinito nella campagna secondaria e nella campagna principale, in modo da poter sovrascrivere il valore della campagna punteggio secondario per le campagne principali (vedi di seguito un esempio visivo)
* Le campagne eseguibili possono essere richiamate fino a tre livelli (ad esempio, Campagna principale > Figlio > Figlio)

>[!CAUTION]
>
>Non lasciare mai i tuoi elenchi avanzati per le campagne eseguibili non validi. In caso contrario, _nessuno_ sarà idoneo. Si consiglia di creare risorse di elenchi avanzati separate, definirle completamente e assicurarsi che siano valide. Quindi, utilizza il filtro &quot;Membro di elenco avanzato&quot; nella campagna eseguibile in modo da poter scambiare la definizione dell’elenco avanzato.

## Esempio di ereditarietà del token {#token-inheritance-example}

Di seguito è riportato un esempio visivo di Ereditarietà token in una campagna eseguibile e due campagne principali: una con il contesto del token impostato su **[!UICONTROL True]** e l&#39;altra su **[!UICONTROL False]**.

Campagna figlio con un punteggio di modifica tokenizzato.

![](assets/execute-campaign-3.png)

La campagna per bambini è My Tokens (I miei token).

![](assets/execute-campaign-4.png)

### Esempio 1 - True {#example-one-true}

Nel passaggio di flusso Esegui campagna della prima campagna principale, &quot;[!UICONTROL Use Parent Campaign Token Context]&quot; è impostato su **[!UICONTROL True]**.

![](assets/execute-campaign-5.png)

La campagna principale è My Tokens.

![](assets/execute-campaign-6.png)

I risultati: punteggio cambiato di +10.

![](assets/execute-campaign-7.png)

### Esempio 2: False {#example-two-false}

Nel passaggio del flusso Esegui campagna della seconda campagna principale, &quot;Usa contesto token campagna principale&quot; è impostato su **False**.

![](assets/execute-campaign-8.png)

La campagna principale è My Tokens.

![](assets/execute-campaign-9.png)

Il punteggio dei risultati: è rimasto invariato, perché è stato utilizzato il valore di punteggio della campagna secondaria, +0.

![](assets/execute-campaign-10.png)
