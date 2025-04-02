---
description: Funzioni GenAI - Documentazione Marketo - Documentazione del prodotto
title: Funzioni GenAI
feature: Interactive Webinars
hide: true
hidefromtoc: true
exl-id: 3e0a41b0-7ff3-4676-bafc-4e7a0725a737
source-git-commit: 374226d3b12cdffe1d0f2e04a1cb00d2f3135d22
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Funzioni GenAI {#gen-ai-features}

Genera automaticamente capitoli e riepiloghi per i webinar registrati, rendendoli più accessibili e facili da consultare per il pubblico.

* **Generazione automatica dei capitoli**: la tecnologia basata sull&#39;intelligenza artificiale crea capitoli per il contenuto del webinar.

* **Riepilogo generato da IA**: ottieni un riepilogo testuale automatico del tuo webinar.

* **Contenuto modificabile**: se necessario, modifica i capitoli e i riepiloghi generati utilizzando le funzionalità di modifica manuali e basate su IA.

* **Integrazione semplificata**: è possibile aggiungere facilmente capitoli e riepiloghi alle pagine di destinazione copiando il codice HTML nell&#39;editor di pagine Web desiderato.

## Abilita GenAI {#enable-genai}

>[!PREREQUISITES]
>
>Prima di utilizzare queste funzioni, devi accettare i termini e le condizioni di Adobe GenAI. Se non lo hai ancora fatto, contatta il team dell’account di Adobe (il tuo Account Manager) per maggiori dettagli.

Dopo aver accettato i termini e le condizioni di Adobe GenAI, il passaggio successivo consiste nell’abilitarli per i singoli utenti. A tale scopo, passare a **[!UICONTROL Admin]** > **[!UICONTROL Interactive Webinars]** e selezionare gli utenti che devono avere accesso a GenAI.

![](assets/gen-ai-features-1.png){width="600" zoomable="yes"}

## Come accedere {#how-to-access}

1. Vai alla pagina della panoramica del webinar nei webinar interattivi di Marketo Engage.

1. Dopo aver condotto il webinar on-demand, attendi 30-60 minuti per consentire all’intelligenza artificiale di elaborare la registrazione. Il pulsante Genera diventa cliccabile quando è disponibile.

1. Fai clic su **[!UICONTROL Generate]**.

   ![](assets/gen-ai-features-2.png){width="800" zoomable="yes"}

1. Viene visualizzata una nuova scheda con i capitoli generati dall’intelligenza artificiale e un riepilogo di testo.

## Modificare il contenuto generato {#edit-generated-content}

1. Esamina i capitoli e il riepilogo generati.

1. Se sono necessarie modifiche, fare clic sul pulsante **[!UICONTROL Edit]**.

   Apportare modifiche:

   * Modifica il testo nel riepilogo e/o nei titoli dei capitoli.

   * Se necessario, regola i timestamp modificando i valori nei campi timestamp.

   * Eliminare i capitoli indesiderati selezionandoli e facendo clic su **[!UICONTROL Delete]**.

   * Unire due capitoli consecutivi selezionandoli e facendo clic su **[!UICONTROL Merge]**.

      * IA genera un capitolo composito composto dai due capitoli selezionati

      * Per unire più capitoli, è necessario eseguire due operazioni alla volta

     ![](assets/gen-ai-features-3.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >* Se lo desideri, puoi valutare la qualità dei capitoli/riepilogo generati con le icone _miniature_ ![miniature verso l&#39;alto](assets/icon-thumbs-up.png) o _miniature verso il basso_ ![miniature verso il basso](assets/icon-thumbs-down.png). Puoi anche segnalare eventuali contenuti problematici facendo clic sull&#39;icona del contrassegno ![icona Contrassegno](assets/icon-flag.png).
   >
   >* Se non si è soddisfatti del riepilogo iniziale, è possibile fare clic sul pulsante **[!UICONTROL Regenerate summary]** per generare un&#39;altra versione.

1. Salva le modifiche facendo clic sul pulsante **[!UICONTROL Save]** in alto a destra dello schermo.

## Utilizzare i contenuti generati {#use-generated-content}

Dopo aver copiato il contenuto che desideri utilizzare, incollalo nell’editor desiderato (ad esempio, l’editor per pagine di destinazione di Marketo Engage) e apporta le eventuali modifiche necessarie.

### Riepilogo {#summary}

**Copia HTML** - Fare clic sul pulsante **[!UICONTROL Copy HTML]** per ottenere tutto il testo, completo di formattazione del codice HTML all&#39;interno di una tabella.

**Solo testo** - Se desideri solo il testo, evidenzialo e seleziona Ctrl/Comando+C (o fai clic con il pulsante destro del mouse) per copiarlo.

### Capitoli {#chapters}

**Copia HTML** - Fare clic sul pulsante **[!UICONTROL Copy HTML]** per formattare tutta la registrazione e i relativi capitoli all&#39;interno di un lettore video.

## Aspetti da considerare {#things-to-note}

* L’eliminazione o l’unione di capitoli influisce solo sullo stack dei capitoli, non sul contenuto video stesso. Queste azioni sono permanenti.

* Le funzioni GenAI sono flessibili e possono essere utilizzate con vari editor di pagine web, non solo con quelli di Marketo Engage.

* Visualizza sempre in anteprima le modifiche per garantire la funzionalità e l&#39;aspetto desiderati.

* Eliminando il webinar viene eliminato anche il contenuto GenAI.

* Se desideri eliminare il contenuto GenAI senza eliminare il webinar, rivolgiti al team dell&#39;account di Adobe (il tuo Account Manager) o invia una richiesta di eliminazione dati a: `marketo-webinar-genai-alerts@adobe.com`.
