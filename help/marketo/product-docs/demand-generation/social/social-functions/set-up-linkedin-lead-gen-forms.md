---
unique-page-id: 12976798
description: Configurare LinkedIn Lead Gen Forms - Documentazione Marketo - Documentazione del prodotto
title: Configurare LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: 94ca714d038863ad801551960c66086ea47e6b10
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Configurare LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Utilizza LinkedIn Lead Gen Forms per eseguire campagne pubblicitarie in LinkedIn e generare lead per Marketo.

>[!IMPORTANT]
>
>LinkedIn sta aggiornando le API di marketing utilizzate dalle integrazioni Marketo Engage LinkedIn. Per evitare interruzioni del servizio, queste modifiche richiederanno la riautenticazione di tutti i servizi LinkedIn LaunchPoint nel menu **Amministratore** > **LaunchPoint** tra il 7 giugno e il 15 dicembre 2024. Per ulteriori informazioni, vedere le [Domande frequenti sulla migrazione](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.

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

1. Immetti un **Nome visualizzato** per il servizio, seleziona il servizio **LinkedIn Lead Gen** dall&#39;elenco a discesa e fai clic su **Avanti**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo apre una nuova scheda nello stesso browser a [linkedin.com](https://www.linkedin.com). Accedi a LinkedIn utilizzando l’account che desideri utilizzare per l’integrazione.

   >[!NOTE]
   >
   >L’account LinkedIn deve poter accedere a tutti gli account aziendali LinkedIn per i quali stai creando campagne sponsorizzate.

   ![](assets/linkedin-login.png)

1. Dopo aver effettuato l&#39;accesso a LinkedIn, tornare a Marketo e fare clic su **Autorizza**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Quando richiesto, fare clic su **Consenti** per accettare l&#39;installazione dell&#39;app Marketo in LinkedIn.

   ![](assets/linkedin-marketo-allow.png)

1. Noterai che ora sei autorizzato. Fai clic su **Avanti**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >Il servizio scade automaticamente un anno dopo l’autorizzazione. Per recuperare l&#39;accesso, fai clic su **Riautorizza**. Potrebbe essere necessario reimmettere la password di LinkedIn, a seconda delle impostazioni del browser.

1. Seleziona gli account da cui vuoi che i lead gen di LinkedIn vengano inseriti in Marketo e fai clic su **Avanti**.

   >[!TIP]
   >
   >Se gli account aziendali previsti non sono visualizzati, verificare che l&#39;account LinkedIn dell&#39;utente che si sta autorizzando disponga delle autorizzazioni Lead Gen Form Manager per l&#39;account aziendale in LinkedIn.

   ![](assets/linkedin-pages-to-capture.png)

1. Per accettare le mappature predefinite dei campi da LinkedIn a Marketo, fai clic su **Crea**. Se desideri modificare la mappatura di campo predefinita, rimuovere una mappatura di campo o aggiungere una nuova mappatura di campo, puoi farlo in base al campo, tramite la finestra modale seguente.

   >[!CAUTION]
   >
   >Marketo supporta la mappatura di due campi di LinkedIn in un singolo campo di Marketo, **ma solo quando** i due campi di LinkedIn non si trovano nello stesso modulo. Se si esegue il mapping di due campi dello stesso modulo di LinkedIn a un singolo campo di Marketo, è possibile che l&#39;immissione del database di Marketo non venga eseguita correttamente.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Solo i campi LinkedIn già salvati in un [modello di modulo](https://www.linkedin.com/help/lms/answer/79634) in LinkedIn Campaign Manager verranno visualizzati come campi LinkedIn che è possibile mappare ai campi Marketo.

   ![](assets/linkedin-installed-services.png)

Ben fatto! Le persone che inviano i moduli LinkedIn Lead Gen inizieranno a fluire in Marketo man mano che esegui campagne di successo sul lato LinkedIn.

>[!NOTE]
>
>Puoi autorizzare un solo account utente di LinkedIn. Se disponi di più account aziendali da collegare a Marketo, accertati che l’account LinkedIn dell’utente che viene autorizzato disponga delle autorizzazioni Lead Gen Form Manager per l’account Business in LinkedIn.

>[!MORELIKETHIS]
>
>[Utilizzare i filtri e i trigger di LinkedIn Lead Gen Form in una campagna avanzata](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
