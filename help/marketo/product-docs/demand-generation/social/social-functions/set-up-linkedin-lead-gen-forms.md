---
unique-page-id: 12976798
description: Impostare LinkedIn Lead Gen Forms - Documenti Marketo - Documentazione del prodotto
title: Imposta LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Imposta LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Utilizza LinkedIn Lead Gen Forms per eseguire campagne pubblicitarie in LinkedIn e generare lead per Marketo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai a Marketo **Amministratore**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vai a **LaunchPoint**, fai clic su **Nuovo** e seleziona **Nuovo servizio**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Inserisci un **Nome visualizzato** per il servizio, seleziona la **Gen. linkedIn** dal menu a discesa e fai clic su **Successivo**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo apre una nuova scheda nello stesso browser in [linkedin.com](https://www.linkedin.com). Accedi a LinkedIn utilizzando l’account che desideri utilizzare per l’integrazione.

   >[!NOTE]
   >
   >L&#39;account LinkedIn deve poter accedere a tutti gli account LinkedIn Business per i quali stai creando campagne sponsorizzate.

   ![](assets/linkedin-login.png)

1. Dopo aver effettuato l’accesso a LinkedIn, torna a Marketo e fai clic su **Autorizzare**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Quando richiesto, fai clic su **Consenti** per accettare l’installazione dell’app Marketo in LinkedIn.

   ![](assets/linkedin-marketo-allow.png)

1. Noterai che ora sei autorizzato. Fai clic su **Successivo**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >Il servizio scade automaticamente un anno dopo l&#39;autorizzazione. Per recuperare l&#39;accesso, fai clic su **Riautorizzare**. Potrebbe essere necessario reimmettere la password LinkedIn, a seconda delle impostazioni del browser.

1. Seleziona gli account da cui desideri che i lead Gen LinkedIn entrino in Marketo e fai clic su **Successivo**.

   >[!TIP]
   >
   >Se non vengono visualizzati gli account aziendali previsti, assicurarsi che l&#39;account LinkedIn dell&#39;utente autorizzato disponga delle autorizzazioni per lead Gen Form Manager per l&#39;account aziendale in LinkedIn.

   ![](assets/linkedin-pages-to-capture.png)

1. Per accettare le mappature dei campi predefinite da LinkedIn a Marketo, fai clic su **Crea**. Se desideri modificare la mappatura campo predefinita, rimuovere una mappatura campo o aggiungere una nuova mappatura campo, puoi farlo a livello di campo tramite il modale seguente.

   >[!CAUTION]
   >
   >Marketo supporta la mappatura di due campi LinkedIn a un singolo campo Marketo, **ma solo quando** i due campi LinkedIn non si trovano nello stesso modulo. Se si mappano due campi dallo stesso modulo LinkedIn a un singolo campo Marketo, l&#39;accesso al database Marketo potrebbe non riuscire.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Solo i campi LinkedIn già salvati in un [modello di modulo](https://www.linkedin.com/help/lms/answer/79634) in LinkedIn Campaign Manager viene visualizzato come Campi LinkedIn che possono essere mappati su campi Marketo.

   ![](assets/linkedin-installed-services.png)

Ben fatto! Le persone che inviano i moduli LinkedIn Lead Gen inizieranno a fluire in Marketo durante l’esecuzione di campagne di successo sul lato LinkedIn.

>[!NOTE]
>
>Puoi autorizzare un solo account utente LinkedIn. Se disponi di più account aziendali che desideri collegare a Marketo, assicurati che l’account LinkedIn dell’utente autorizzato disponga delle autorizzazioni per lead Gen Form Manager per l’account aziendale in LinkedIn.

>[!MORELIKETHIS]
>
>[Utilizzare filtri e attivatori per moduli lead Gen LinkedIn in una campagna avanzata](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
