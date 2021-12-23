---
unique-page-id: 3571805
description: Passaggio 1 di 3 - Installare la soluzione Marketo (2011 On-Premises) - Marketo Docs - Documentazione del prodotto
title: Passaggio 1 di 3 - Installare la soluzione Marketo (2011 On-Premises)
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
source-git-commit: 2568d3414c8aaec882b79442f6312bae3b9514ab
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Passaggio 1 di 3: Installare la soluzione Marketo (On-Premises 2011) {#step-of-install-the-marketo-solution-on-premises}

Prima di poter sincronizzare Microsoft Dynamics On-Premises e Marketo, è necessario installare la soluzione Marketo in Dynamics.

>[!NOTE]
>
>Dopo aver sincronizzato Marketo con un CRM, non puoi eseguire una nuova sincronizzazione senza sostituire l&#39;istanza.

>[!PREREQUISITES]
>
>Devi avere [Implementazione di Internet Facing](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) con [Servizi federativi Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 o 3.0 (ADFS) configurati. **Nota**: Il documento IFD viene scaricato automaticamente quando fai clic sul collegamento.
>
>[Scarica la soluzione Marketo per la gestione dei lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) prima di iniziare.

>[!NOTE]
>
>**Autorizzazioni per l’amministrazione di Dynamics richieste.**
>
>Per eseguire questa sincronizzazione è necessario disporre dei privilegi di amministratore CRM.

1. Accedi a **Dynamics**, seleziona **Impostazioni** nel menu in basso a sinistra.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Seleziona **Soluzioni** nell&#39;albero.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Fai clic su **Importa**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Fai clic su **Sfoglia**. Seleziona la soluzione Marketo Lead Management [scaricato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Fai clic su **Successivo**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Visualizza le informazioni sulla soluzione e fai clic su **Visualizza i dettagli del pacchetto della soluzione**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Dopo aver controllato tutti i dettagli, fai clic su **Chiudi**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Nella pagina Informazioni sulla soluzione , fai clic su **Successivo**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Assicurati che la casella di controllo dell&#39;opzione Messaggio SDK sia selezionata. Fai clic su **Successivo**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Sarà necessario abilitare i pop-up sul browser per completare il processo di installazione.

1. Ora attendi il completamento dell’importazione. Alzati e fai delle distese.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Fai clic su **Chiudi**.

   >[!NOTE]
   >
   >È possibile che venga visualizzato un messaggio che indica &quot;Gestione lead Marketo completata con un avviso&quot;. Ciò è pienamente atteso.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Gestione lead Marketo verrà ora visualizzata nella pagina **Tutte le soluzioni** pagina.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Seleziona Gestione lead Marketo e fai clic su **Pubblica Tutte Le Personalizzazioni.**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

Non era male giusto? Avanti, continuerò a passarvi attraverso il resto.

>[!CAUTION]
>
>La disattivazione di uno qualsiasi dei processi di messaggistica SDK di Marketo provocherà un&#39;installazione non funzionante.

>[!MORELIKETHIS]
>
>[Passaggio 2 di 3: Configurazione dell’utente di sincronizzazione Marketo in Dynamics (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-2-of-3-set-up.md)
