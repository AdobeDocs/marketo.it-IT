---
title: Understanding-my-tokens
description: Informazioni sui token
exl-id: d56748e2-d742-45dd-96a8-dd80e30d9d8b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Informazioni sui token

<br> 

I miei token sono variabili personalizzate che puoi creare e utilizzare nei tuoi programmi o cartelle di campagne. Hanno questo aspetto: `{{_my.Name of Token_}}`

## Esempi

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

Per accedere e creare i token personali, seleziona la cartella del programma o della campagna e vai alla scheda [!UICONTROL My Tokens] . Trascina e rilascia un token nell’ area di lavoro [!UICONTROL Local Tokens].

![Immagine uno](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-1.png)

>[!CAUTION]
>
>I nomi dei token personali non possono essere modificati dopo il salvataggio, quindi scegli con attenzione.

>[!NOTE]
>
>I miei token non verranno risolti quando invii un’e-mail da Sales Insight in Microsoft Dynamics o Salesforce; verranno compilati solo i token standard (Lead, Azienda, ecc.). Tuttavia, i valori predefiniti per i token funzioneranno.

>[!NOTE]
>
>I token di collegamento non funzionano nelle e-mail di solo testo.

## Nidificazione dei token

Quando si crea un nuovo token, è possibile farvi riferimento da altri oggetti nella struttura. È possibile sostituire le variabili globali ai livelli inferiori nella struttura. Esiste una struttura di denominazione per la creazione del token per una gestione semplice.

* **Token locale:** il token è stato creato direttamente in quel programma o cartella.
* **[Token ignorato:](/help/sky/override-an-inherited-my-token.md)** il token è stato ereditato, ma è stata fatta un&#39;eccezione in questo programma o cartella.
* **Token ereditato:** il token è stato creato nella struttura in un punto qualsiasi di un programma o di una cartella di livello superiore.

Puoi trovare questi tre tipi sotto la scheda **[!UICONTROL My Tokens]** nella cartella del programma o della campagna.

![Immagine 2](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-2.png)

Lo spostamento di programmi e cartelle influisce anche sui token. Controlla sempre se i riferimenti non sono interrotti durante lo spostamento.

>[!NOTE]
>
>Se l’e-mail inviata da un programma di coinvolgimento è un’e-mail figlia di un programma predefinito (ovvero non locale per il programma di coinvolgimento), tutti i token personali utilizzati nell’e-mail vengono risolti dal programma predefinito in cui risiede l’e-mail figlio.

## Utilizzo token

Seleziona un token, quindi fai clic sull’icona di utilizzo nell’angolo in alto a destra per visualizzare un elenco delle risorse che contengono tale token.

![Immagine tre](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-3.png)

![Immagine quattro](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-4.png)

**Immersione profonda**

Ulteriori informazioni su ciascuno dei token personali:

* [Campaign CRM](/help/sky/my-token-crm-campaign.md)
* [Data](/help/sky/my-token-date.md)
* [File di calendario](/help/sky/my-token-calendar-file.md)
* [Immagine](/help/sky/my-token-image.md)
* [Collegamento](/help/sky/my-token-link.md)
* [Numero](/help/sky/my-token-number.md)
* [Rich Text](/help/sky/my-token-rich-text.md)
* [Punteggio](/help/sky/my-token-score.md)
* [Script e-mail](/help/sky/my-token-email-script.md)
* [Testo](/help/sky/my-token-text.md)
