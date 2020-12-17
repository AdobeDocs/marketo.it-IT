---
title: understanding-my-token
description: Informazioni sui token personali
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---


# Informazioni sui token personali

<br> 

I miei token sono variabili personalizzate che puoi creare e utilizzare nei tuoi programmi o nelle cartelle delle campagne. Hanno questo aspetto: `{{_my.Name of Token_}}`

## Esempi

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

Per accedere e creare i Token personali, seleziona la cartella del programma o della campagna e vai alla scheda [!UICONTROL My Tokens]. Trascina e rilascia qualsiasi token sul quadro [!UICONTROL Local Tokens].

![Immagine uno](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-1.png)

>[!CAUTION]
>
>I nomi dei Token personali non possono essere modificati dopo che sono stati salvati, quindi scegli attentamente.

>[!NOTE]
>
>I miei token non verranno risolti quando si invia un&#39;e-mail da Sales Insight in Microsoft Dynamics o Salesforce; verranno compilati solo i token standard (Lead, Società, ecc.). Tuttavia, i valori predefiniti per i token funzioneranno.

>[!NOTE]
>
>I token di collegamento non funzionano nelle e-mail di solo testo.

## Nidificazione dei token

Quando si crea un nuovo token, è possibile farvi riferimento da altri oggetti della struttura. È possibile ignorare le variabili globali a livelli inferiori nella struttura. Esiste una struttura di denominazione in cui è stato creato il token per una gestione semplice.

* **Token locale:** il token è stato creato direttamente in tale programma o cartella.
* **[Token ignorato:](/help/sky/override-an-inherited-my-token.md)** il token è stato ereditato, ma è stata fatta un&#39;eccezione in questo programma o in questa cartella.
* **Token ereditato:** il token è stato creato nella struttura ad albero in un punto qualsiasi di un programma o una cartella di livello superiore.

Questi tre tipi si trovano nella scheda **[!UICONTROL My Tokens]** nella cartella del programma o della campagna.

![Immagine due](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-2.png)

Lo spostamento di programmi e cartelle influisce anche sui token. Controllate sempre per essere certi che i riferimenti non vengano interrotti durante lo spostamento.

>[!NOTE]
>
>Se l&#39;e-mail inviata da un programma di partecipazione è un&#39;e-mail figlia di un programma predefinito (ovvero, non locale al programma di coinvolgimento), tutti i Token utente utilizzati nell&#39;e-mail vengono risolti dal programma predefinito in cui risiede l&#39;e-mail del bambino.

## Utilizzo token

Selezionate un token, quindi fate clic sull’icona di utilizzo nell’angolo in alto a destra per visualizzare un elenco delle risorse che contengono tale token.

![Immagine tre](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-3.png)

![Immagine quattro](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-4.png)

**Tubo profondo**

Ulteriori informazioni su ciascuno dei Token personali:

* [Campaign CRM](/help/sky/my-token-crm-campaign.md)
* [Data](/help/sky/my-token-date.md)
* [File calendario](/help/sky/my-token-calendar-file.md)
* [Immagine](/help/sky/my-token-image.md)
* [Collegamento](/help/sky/my-token-link.md)
* [Numero](/help/sky/my-token-number.md)
* [Rich Text](/help/sky/my-token-rich-text.md)
* [Punteggio](/help/sky/my-token-score.md)
* [Script e-mail](/help/sky/my-token-email-script.md)
* [Testo](/help/sky/my-token-text.md)
