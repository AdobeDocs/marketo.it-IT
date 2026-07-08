---
solution: Marketo Engage
product: marketo
title: Conformità alle linee guida CNIL - Tracciamento dell’apertura condizionale delle e-mail
description: Scopri come configurare Marketo Engage per la conformità CNIL utilizzando un campo booleano personalizzato per instradare il tracciamento delle e-mail aperte in base allo stato di consenso di ogni persona.
level: Beginner, Intermediate
feature: Email Designer
hide: true
source-git-commit: c0c8e88ae6357c4bf75437e1bbc7fe0d6bce1012
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Conformità alle linee guida CNIL: tracciamento dell’apertura condizionale delle e-mail {#cnil}

Scopri come configurare Marketo Engage per rispettare il consenso degli utenti finali per il tracciamento dell’apertura delle e-mail (pixel), in conformità alle linee guida CNIL (COMMUNITY LINK). L’approccio utilizza un campo booleano personalizzato per determinare quale variante e-mail riceve una persona, una con il tracciamento aperto abilitato o una con esso disabilitato.

## Passaggio 1: creare un campo booleano personalizzato {#custom-field}

1. Nell&#39;area **Amministratore**, fare clic su **Gestione campi** e selezionare **Nuovo campo personalizzato**.

   ![](assets/cnil-1.png)

1. Per _Oggetto_, scegli **Persona**. Per _Type_, scegli **Boolean**. Per _Name_, immetti &quot;Email Pixel Tracking&quot; (il nome API si popola automaticamente). Fai clic su **Crea**.

   ![](assets/cnil-2.png)

## Passaggio 2: compilare il campo del consenso {#populate}

1. Imposta il valore del campo Tracciamento pixel e-mail per ogni persona tramite importazione dati (sincronizzazione API o [caricamento CSV](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people){target="_blank"}).

   ![](assets/cnil-3.png)

1. Assicurati che il campo personalizzato sia mappato correttamente.

   ![](assets/cnil-4.png)

>[!NOTE]
>
>In futuro, potrai acquisire i dati direttamente durante la compilazione di un modulo, consentendo all’utente di dare o rinunciare al tracciamento delle aperture dei messaggi e-mail.

## Passaggio 3: creare varianti e-mail {#variants}

Crea due e-mail. Il tracciamento dell’apertura delle e-mail è abilitato per impostazione predefinita sia per E-mail Designer che per l’editor e-mail legacy.

* **E-mail uno (tracciamento delle aperture abilitato)**: dopo la creazione dell&#39;e-mail, non è richiesta alcuna ulteriore azione. Mantieni il tracciamento aperto abilitato.

* **E-mail due (tracciamento delle aperture disabilitato)**: Clona e-mail uno e disabilita il tracciamento delle aperture.

  ![](assets/cnil-5.png)

In E-mail Designer, la casella di controllo **Disattiva tracciamento aperto** si trova nella scheda _Dettagli_ del riquadro _Riepilogo_ a destra dell&#39;e-mail. Nell&#39;editor e-mail legacy, la casella di controllo **Disattiva tracciamento aperto** si trova nel menu _Impostazioni e-mail_.

**E-mail Designer**

![](assets/cnil-6.png){width="800" zoomable="yes"}

**Editor e-mail legacy**

![](assets/cnil-7.png){width="800" zoomable="yes"}

## Passaggio 4: configurare Smart Campaign {#smart-campaign}

[Crea una campagna avanzata](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign){target="_blank"} per determinare quale e-mail riceve ogni persona.

1. Nella scheda _Flusso_ della tua Smart Campaign, inserisci il passaggio di flusso **Invia e-mail**.

   ![](assets/cnil-8.png){width="800" zoomable="yes"}

1. Nel passaggio del flusso, fare clic su **Aggiungi scelta**. Nella scelta 1, impostare **if** su _Tracciamento pixel e-mail_, impostare l&#39;operatore su _is_ e impostare il valore su _false_. Per **E-mail**, seleziona _E-mail due_.

1. In Scelta predefinita, impostare **E-mail** su _E-mail uno_.

   ![](assets/cnil-9.png)

In questo modo le persone che non hanno acconsentito al tracciamento aperto ricevono l’e-mail non tracciata, mentre le persone che hanno acconsentito ricevono l’e-mail tracciata standard.
