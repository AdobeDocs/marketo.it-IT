---
description: Scopri come i metadati C2PA vengono automaticamente allegati alle immagini generate dall’intelligenza artificiale in Marketo Engage, conservati tramite modifiche e utilizzati per la provenienza dei contenuti.
title: Metadati C2PA in Marketo Engage
level: Beginner, Intermediate
feature: Email Designer
source-git-commit: 10781cbfd51019a2e4af346803a2e35ef40855d0
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 2%

---

# Metadati C2PA in Marketo Engage

Nuove leggi stanno emergendo sulla trasparenza generativa dell’intelligenza artificiale e Adobe sta lavorando per soddisfare i requisiti applicabili in tutte le giurisdizioni. I metadati C2PA sono lo strumento di provenienza utilizzato da Adobe per soddisfare i requisiti di queste normative.

I metadati C2PA sono metadati invisibili e duraturi che registrano il modo in cui un contenuto è stato creato o modificato. Quando si genera o si modifica un&#39;immagine con strumenti di intelligenza artificiale generativi in Marketo Engage, i metadati C2PA vengono automaticamente allegati all&#39;immagine (non è richiesta alcuna azione da parte dell&#39;utente). Si tratta di informazioni crittografate, in grado di evidenziare eventuali manomissioni, che possono aiutare gli utenti a comprendere la linea di contenuti e garantire l’integrità delle risorse del marchio. Queste informazioni includono:

* **Emittente o firmatario**: informazioni sull&#39;entità o sulla società che ha emesso la firma digitale per certificare o firmare la risorsa.
* **Data problema**: data in cui i metadati C2PA sono stati applicati alla risorsa.
* **Credito e utilizzo**: informazioni sul produttore della risorsa, tra cui nome, handle per social media o altre informazioni relative all&#39;identità.
* **Processo**: record di eventuali modifiche apportate alla risorsa.
* **Dettagli dispositivo**: informazioni sull&#39;app o sul dispositivo utilizzato per creare o modificare la risorsa.
* **Strumento di intelligenza artificiale utilizzato**: se per creare la risorsa è stata utilizzata l&#39;intelligenza artificiale generativa, è possibile includere il nome del modello utilizzato.
* **Altre informazioni importanti**: sono inclusi anche dati aggiuntivi per offrire più contesto sulla cronologia di una risorsa.

## Azioni che associano metadati C2PA

La tabella seguente riepiloga quando vengono allegati metadati C2PA, in base all’azione eseguita nella generazione di immagini in Marketo Engage.

| Azione | Descrizione | Metadati C2PA allegati? | Esempio di caso d’uso |
|---|---|---|---|
| **Utilizza lo strumento &#39;Genera immagine&#39;** | Create una nuova immagine da un prompt di testo, da un&#39;immagine di riferimento o generate un&#39;immagine simile. | Sempre. L’immagine viene generata dall’intelligenza artificiale generativa, in modo da trasportare sempre nuovi metadati C2PA. | Un’immagine del banner per una campagna e-mail viene generata da un prompt di testo che descrive l’elemento visivo desiderato. |
| **Ritagliare un&#39;immagine** | Regola un&#39;immagine alle dimensioni richieste. | Solo se l’immagine di origine conteneva già metadati C2PA. Il ritaglio ricrea i pixel dell&#39;immagine, che normalmente cancellano i metadati C2PA, quindi Marketo Engage lo legge dall&#39;immagine sorgente prima del ritaglio, quindi lo ricostruisce e lo ricollega al risultato ritagliato. Il ritaglio stesso non aggiunge una nuova azione di IA generativa, ma mantiene quella esistente. | Un’immagine del banner generata viene ritagliata per adattarla a una pagina web: i metadati C2PA vengono conservati attraverso il ritaglio. Una foto stock caricata, utilizzata come sfondo di notifica push, viene ritagliata per adattarsi allo schermo: poiché la foto stock non comporta alcuna azione AI generativa, non vengono creati metadati C2PA. |
| **Aggiungi una sovrapposizione di testo** | Rendering del testo generato sopra un&#39;immagine di sfondo. | Solo se l’immagine di sfondo conteneva già metadati C2PA. Il rendering della sovrapposizione produce una nuova immagine dallo sfondo più il testo, che normalmente cancella i metadati C2PA, in modo che Marketo Engage lo legga in anticipo dall&#39;immagine di sfondo, quindi lo ricostruisce e lo ricollega al risultato. Il passaggio di sovrapposizione non aggiunge una nuova azione di IA generativa. | Un titolo promozionale viene riprodotto come sovrapposizione di testo su un’immagine di sfondo generata per una pagina di destinazione: i metadati C2PA dell’immagine di sfondo vengono mantenuti. |

## Tipi di contenuto e ambito

**Immagini**: coperte. I metadati C2PA vengono allegati quando le immagini vengono generate con intelligenza artificiale generativa e vengono conservati mediante le operazioni di ritaglio e sovrapposizione del testo eseguite durante la generazione delle immagini in Marketo Engage.

**Testo**: non applicabile. Gli output di solo testo per la generazione di immagini in Marketo Engage, come la generazione di copie, la traduzione e i suggerimenti di allineamento del brand, non richiedono metadati C2PA.

## Cosa succede quando il contenuto si sposta

Marketo Engage conserva i metadati C2PA associati alle risorse immagine supportate. Se un’immagine contiene metadati C2PA quando viene importata in Marketo Engage, questi vengono conservati quando la risorsa viene utilizzata nei contenuti della campagna generata e nelle esperienze e-mail in uscita.

## Risorse aggiuntive

* [Trasparenza dei contenuti di IA generativa](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/overview/content-transparency){target="_blank"}
* [Linee guida utente per l’intelligenza artificiale generativa di Adobe Experience Cloud](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}
* [Guardrail e limitazioni](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/generate-content/gs-generative#generative-guardrails){target="_blank"}
