---
unique-page-id: 12976798
description: Configurare LinkedIn Lead Gen Forms - Documentazione Marketo - Documentazione del prodotto
title: Configurare LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: e1254c8156557b27d066a4482076becbd03fc774
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Configurare LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Utilizza LinkedIn Lead Gen Forms per eseguire campagne pubblicitarie in LinkedIn e generare lead per Marketo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>Un lead LinkedIn non entra nel Marketo Engage se corrisponde a un record persona esistente in Marketo associato a un record azienda creato utilizzando le API aziendali e la sottoscrizione Marketo non è connessa a un CRM.

1. Vai a Marketo **Amministratore**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vai a **LaunchPoint**, fai clic su **Nuovo** e seleziona **Nuovo servizio**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Immetti un **Nome visualizzato** per il servizio, seleziona **LinkedIn Lead Gen** dal menu a discesa, quindi fai clic su **Successivo**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo apre una nuova scheda nello stesso browser per [linkedin.com](https://www.linkedin.com). Accedi a LinkedIn utilizzando l’account che desideri utilizzare per l’integrazione.

   >[!NOTE]
   >
   >L’account LinkedIn deve poter accedere a tutti gli account aziendali LinkedIn per i quali stai creando campagne sponsorizzate.

   ![](assets/linkedin-login.png)

1. Dopo aver effettuato l’accesso a LinkedIn, torna a Marketo e fai clic su **Autorizza**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Quando richiesto, fai clic su **Consenti** per accettare l’installazione dell’app Marketo in LinkedIn.

   ![](assets/linkedin-marketo-allow.png)

1. Noterai che ora sei autorizzato. Fai clic su **Avanti**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >Il servizio scade automaticamente un anno dopo l’autorizzazione. Per recuperare l’accesso, fai clic su **Autorizza nuovamente**. Potrebbe essere necessario reimmettere la password di LinkedIn, a seconda delle impostazioni del browser.

1. Seleziona gli account da cui desideri che i lead Gen di LinkedIn vengano inseriti in Marketo e fai clic su **Successivo**.

   >[!TIP]
   >
   >Se gli account aziendali previsti non sono visualizzati, verificare che l&#39;account LinkedIn dell&#39;utente che si sta autorizzando disponga delle autorizzazioni Lead Gen Form Manager per l&#39;account aziendale in LinkedIn.

   ![](assets/linkedin-pages-to-capture.png)

1. Per accettare le mappature predefinite dei campi da LinkedIn a Marketo, fai clic su **Crea**. Se desideri modificare la mappatura di campo predefinita, rimuovere una mappatura di campo o aggiungere una nuova mappatura di campo, puoi farlo in base al campo, tramite la finestra modale seguente.

   >[!CAUTION]
   >
   >Marketo supporta la mappatura di due campi LinkedIn in un singolo campo Marketo, **ma solo quando** i due campi di LinkedIn non si trovano nello stesso modulo. Se si esegue il mapping di due campi dello stesso modulo di LinkedIn a un singolo campo di Marketo, è possibile che l&#39;immissione del database di Marketo non venga eseguita correttamente.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Solo i campi LinkedIn già salvati in un [modello di modulo](https://www.linkedin.com/help/lms/answer/79634) in LinkedIn Campaign Manager verranno visualizzati come Campi LinkedIn che possono essere mappati ai campi Marketo.

   ![](assets/linkedin-installed-services.png)

Ben fatto! Le persone che inviano i moduli LinkedIn Lead Gen inizieranno a fluire in Marketo man mano che esegui campagne di successo sul lato LinkedIn.

>[!NOTE]
>
>Puoi autorizzare un solo account utente di LinkedIn. Se disponi di più account aziendali da collegare a Marketo, accertati che l’account LinkedIn dell’utente che viene autorizzato disponga delle autorizzazioni Lead Gen Form Manager per l’account Business in LinkedIn.

>[!MORELIKETHIS]
>
>[Utilizzare i filtri e i trigger per moduli di generazione lead di LinkedIn in una campagna avanzata](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
