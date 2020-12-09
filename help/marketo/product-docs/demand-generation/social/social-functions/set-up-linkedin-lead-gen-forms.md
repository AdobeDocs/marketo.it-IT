---
unique-page-id: 12976798
description: Imposta LinkedIn Lead Gen Forms - Marketo Docs - Documentazione prodotto
title: Imposta LinkedIn Lead Gen Forms
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# Imposta LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Utilizza LinkedIn Lead Gen Forms per eseguire campagne pubblicitarie in LinkedIn e generare lead per Marketo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai ad **Amministratore** Marketo.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vai a **LaunchPoint**, fai clic su **Nuovo** e seleziona **Nuovo servizio**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Immettete un nome **** visualizzato per il servizio, selezionate il servizio **LinkedIn Lead Gen **dall&#39;elenco a discesa, quindi fate clic su **Avanti**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo apre una nuova scheda nello stesso browser su [www.linkedin.com](http://www.linkedin.com). Accedete a LinkedIn utilizzando l&#39;account che desiderate utilizzare per l&#39;integrazione.

   >[!NOTE]
   >
   >L&#39;account LinkedIn deve poter accedere a tutti gli account Business LinkedIn per i quali si creano campagne sponsorizzate.

   ![](assets/linkedin-login.png)

1. Dopo aver effettuato l’accesso a LinkedIn, tornate a Marketo e fate clic su **Autorizza**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Quando richiesto, fare clic su **Consenti **per accettare l&#39;installazione dell&#39;app Marketo in LinkedIn.

   ![](assets/linkedin-marketo-allow.png)

1. Noterete che ora siete autorizzati. Fate clic su **Avanti**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >Il servizio scade automaticamente un anno dopo l&#39;autorizzazione. Per recuperare l’accesso, fate clic su **Riattiva autorizzazione**. A seconda delle impostazioni del browser, potrebbe essere necessario immettere nuovamente la password LinkedIn.

1. Selezionate gli account da cui desiderate che i lead di LinkedIn Lead Gen arrivino a Marketo e fate clic su **Avanti**.

   >[!TIP]
   >
   >Se non vengono visualizzati gli account aziendali previsti, accertatevi che l&#39;account LinkedIn dell&#39;utente autorizzato disponga delle autorizzazioni per il Gestore dei moduli lead Gen per l&#39;account Business di LinkedIn.

   ![](assets/linkedin-pages-to-capture.png)

1. Per accettare le mappature dei campi da LinkedIn a Marketo predefinite, fai clic su **Crea**. Se si desidera modificare la mappatura dei campi predefinita, rimuovere una mappatura dei campi o aggiungere una nuova mappatura dei campi, è possibile eseguire questa operazione in base ai campi utilizzando la modalità indicata di seguito.

   >[!CAUTION]
   >
   >Marketo supporta la mappatura di due campi LinkedIn a un singolo campo Marketo, **ma solo quando** i due campi LinkedIn non si trovano sullo stesso modulo. Se mappate due campi dallo stesso modulo LinkedIn a un singolo campo Marketo, l&#39;accesso al database Marketo potrebbe non riuscire.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Solo i campi LinkedIn che sono già stati salvati in un modello [di](https://www.linkedin.com/help/lms/answer/79634) modulo in Gestione campagne LinkedIn verranno visualizzati come Campi LinkedIn che è possibile mappare ai campi Marketo.

   ![](assets/linkedin-installed-services.png)

Ben fatto! Gli utenti che inviano moduli di LinkedIn Lead Gen inizieranno a far fluire i moduli in Marketo durante l&#39;esecuzione di campagne di successo sul lato LinkedIn.

>[!NOTE]
>
>È possibile autorizzare un solo account utente LinkedIn. Se si dispone di più account Business che si desidera collegare a Marketo, assicurarsi che l&#39;account LinkedIn dell&#39;utente che viene autorizzato disponga delle autorizzazioni per il Gestore dei moduli lead Gen all&#39;account Business in LinkedIn.

>[!MORELIKETHIS]
>
>* [Utilizzare i filtri e gli attivatori per moduli principali LinkedIn in una campagna avanzata](use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)

>



