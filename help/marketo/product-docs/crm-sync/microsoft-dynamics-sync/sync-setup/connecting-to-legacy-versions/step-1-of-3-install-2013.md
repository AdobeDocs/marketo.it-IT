---
unique-page-id: 3571813
description: Passaggio 1 di 3 - Installare la soluzione Marketo in Dynamics (2013 On-Premises) - Marketo Docs - Documentazione del prodotto
title: 'Passaggio 1 di 3: installare la soluzione Marketo in Dynamics (On-Premises 2013)'
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
source-git-commit: 64c5f03bd2320bfbffd257684d1482e995def83a
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Passaggio 1 di 3: Installare la soluzione Marketo in Dynamics (On-Premises 2013) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Prima di poter sincronizzare Microsoft Dynamics On-Premises e Marketo, è necessario installare la soluzione Marketo in Dynamics.

>[!NOTE]
>
>Dopo aver sincronizzato Marketo con un CRM, non puoi eseguire una nuova sincronizzazione senza sostituire l&#39;istanza.

>[!PREREQUISITES]
>
>Devi avere [Implementazione di Internet Facing](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) con [Servizi federativi Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 o 3.0 (ADFS) configurati. Nota: Il documento IFD viene scaricato automaticamente quando fai clic sul collegamento.
>
>[Scarica la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) prima di iniziare.

>[!NOTE]
>
>**Autorizzazioni per l’amministrazione di Dynamics richieste.**
>
>Per eseguire questa sincronizzazione è necessario disporre dei privilegi di amministratore CRM.

1. Accedi a **Dynamics**. Fai clic sul pulsante **Microsoft Dynamics CRM** menu a discesa e seleziona **Impostazioni**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. Sotto **Impostazioni**, seleziona **Soluzioni**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Fai clic su **Importa**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Fai clic su **Sfoglia** e seleziona la [soluzione scaricata](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Fai clic su **Successivo**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Visualizza le informazioni sulla soluzione e fai clic su **Visualizza i dettagli del pacchetto della soluzione**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Dopo aver controllato tutti i dettagli, fai clic su **Chiudi**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Nella pagina Informazioni sulla soluzione , fai clic su **Successivo**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Assicurati che l&#39;opzione SDK sia selezionata. Fai clic su **Importa**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Attendi il completamento dell’importazione.

   >[!TIP]
   >
   >Sarà necessario abilitare i pop-up sul browser per completare il processo di installazione.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Scarica un file di registro (se lo desideri) e fai clic su **Chiudi**.

   >[!NOTE]
   >
   >È possibile che venga visualizzato un messaggio che indica &quot;Gestione lead Marketo completata con un avviso&quot;. Ciò è pienamente atteso.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Gestione lead Marketo verrà ora visualizzata nella pagina **Tutte le soluzioni** pagina.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Seleziona la soluzione Marketo e fai clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

Non era male giusto? Avanti, continuerò a passarvi attraverso il resto.

>[!CAUTION]
>
>La disattivazione di uno qualsiasi dei processi di messaggistica SDK di Marketo provocherà un&#39;installazione non funzionante.

>[!MORELIKETHIS]
>
>[Passaggio 2 di 3: Configura l’utente di sincronizzazione per Marketo (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)
