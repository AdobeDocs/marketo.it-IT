---
description: Installare Marketo per Microsoft Dynamics 2016/Dynamics 365 On-Premises 1 di 3 - Documentazione Marketo - Documentazione del prodotto
title: Installare Marketo per Microsoft Dynamics 2016/Dynamics 365 On-Premises, passaggio 1 di 3
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
source-git-commit: 3fb93520a653109845c3b40aba20304c6163214f
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Passaggio 1 di 3: Configura l’utente di sincronizzazione per Marketo (On-Prem 2016/Dynamics 365 On-Premises) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Prima di poter sincronizzare Microsoft Dynamics 2016 On-Prem/Dynamics 365 con Marketo, è necessario installare la soluzione Marketo in Dynamics.

>[!NOTE]
>
>Dopo aver sincronizzato Marketo con un CRM, non puoi sincronizzare un nuovo CRM con l&#39;istanza Marketo esistente.

>[!PREREQUISITES]
>
>Se utilizzi Microsoft Dynamics On-Premise, devi disporre di [Implementazione di Internet Facing](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) con [Servizi federativi Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS) configurato. Nota: Il documento IFD viene scaricato automaticamente quando fai clic sul collegamento.
>
>[Scarica la soluzione Marketo per la gestione dei lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) prima di iniziare.

>[!NOTE]
>
>**Autorizzazioni per l’amministrazione di Dynamics richieste.**
>
>Per eseguire questa sincronizzazione è necessario disporre dei privilegi di amministratore CRM.

1. Accedi a **Dinamica.** Fai clic sul pulsante **Microsoft Dynamics CRM** menu a discesa e seleziona **Impostazioni**.

   ![](assets/image2015-3-19-8-33-29.png)

1. Sotto **Impostazioni**, seleziona **Soluzioni**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Fai clic su **Importa**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Fai clic su **Sfoglia** e seleziona la soluzione [scaricato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Fai clic su **Successivo**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Visualizza le informazioni sulla soluzione e fai clic su **Visualizza i dettagli del pacchetto della soluzione**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Dopo aver controllato tutti i dettagli, fai clic su **Chiudi**.

   ![](assets/step6.png)

1. Nella pagina Informazioni sulla soluzione , fai clic su **Successivo**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Assicurati che la casella di controllo dell&#39;opzione SDK sia selezionata. Fai clic su **Importa**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Attendi il completamento dell’importazione.

   >[!TIP]
   >
   >Sarà necessario abilitare i pop-up sul browser per completare il processo di installazione.

   ![](assets/image2015-3-11-11-34-9.png)

1. Scarica un file di registro (se lo desideri) e fai clic su **Chiudi**.

   >[!NOTE]
   >
   >È possibile che venga visualizzato un messaggio che indica &quot;Gestione lead Marketo completata con un avviso&quot;. Ciò è pienamente atteso.

   ![](assets/image2015-3-13-9-54-39.png)

1. Gestione lead Marketo verrà ora visualizzata nella pagina **Tutte le soluzioni** pagina.

   ![](assets/image2015-3-19-8-40-38.png)

1. Seleziona la soluzione Marketo e fai clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/image2015-3-19-8-41-21.png)

   Cinque in alto! Installazione completata.

   >[!CAUTION]
   >
   >La disattivazione di uno qualsiasi dei processi di messaggistica SDK di Marketo provocherà un&#39;installazione non funzionante.

   >[!MORELIKETHIS]
   >
   >[Installare Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 2 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
