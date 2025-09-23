---
unique-page-id: 1147108
description: Importare un programma - Documentazione di Marketo - Documentazione del prodotto
title: Importare un programma
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
feature: Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 2%

---

# Importare un programma {#import-a-program}

Un programma può essere importato da un abbonamento Marketo Engage a un altro. Ad esempio, puoi creare un programma in una sandbox e quindi importarlo nel tuo abbonamento live. È inoltre possibile importare un programma predefinito dalla [Libreria programmi di Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/program-library/program-import-library-overview.md){target="_blank"}.

>[!CAUTION]
>
>I programmi che dispongono di elenchi avanzati contenenti un trigger &quot;L’oggetto personalizzato è aggiornato&quot; causeranno l’interruzione dell’importazione. Rimuovi questo trigger da tutti gli elenchi smart prima di seguire i passaggi descritti di seguito.

## Importazione di un programma {#importing-a-program}

1. Vai a **[!UICONTROL Marketing Activities]**.

   ![](assets/import-a-program-1.png)

1. Fai clic sul menu a discesa **[!UICONTROL New]** e seleziona **[!UICONTROL Import Program]**.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >* Importazione programmi è disponibile solo per gli utenti che dispongono di ruoli con l&#39;autorizzazione Importazione programmi abilitata. Ulteriori informazioni sulla gestione di [ruoli utente e autorizzazioni](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.
   >
   >* Per collegare un account sandbox al tuo abbonamento live, contatta il [supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. Selezionare un Marketo **[!UICONTROL Subscription]** e un programma da importare. Fai clic su **[!UICONTROL Next]**.

   ![](assets/import-a-program-3.png)

1. Specificare **[!UICONTROL Campaign Folder]** per il programma importato. Fai clic su **[!UICONTROL Next]**.

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >Assicurarsi che siano selezionate **[!UICONTROL Use default conflict]** regole. Le regole di conflitto sono necessarie quando si importano programmi in un&#39;istanza con risorse con lo stesso nome.

1. Scegliere i dettagli sul conflitto desiderati e fare clic su **[!UICONTROL Next]**.

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >Quando si importa un programma che utilizza i passaggi di flusso personalizzati o le regole di elenchi avanzati derivate da un servizio di passaggi di flusso in un&#39;istanza di destinazione in cui è presente più di un provider di servizi compatibile, all&#39;utente di importazione viene richiesto di assegnare i passaggi o le regole al provider di servizi corretto nell&#39;istanza di destinazione.

1. Visualizza l&#39;anteprima dei dettagli e **[!UICONTROL Import]** il programma.

   ![](assets/import-a-program-6.png)

Al termine dell’importazione riceverai una conferma e-mail.

>[!NOTE]
>
>Dovrai riprogrammare le campagne batch importate e attivare le campagne trigger. Il sistema disattiva automaticamente le pianificazioni delle campagne e attiva le campagne nel programma importato.

## Impatto su Assets esterno durante le importazioni del programma {#impact-on-external-assets-during-program-imports}

I programmi utilizzano risorse esterne come modelli e-mail, modelli di pagina di destinazione, immagini, moduli, token e tag di programma. È possibile configurare la modalità di gestione dei modelli della pagina di destinazione e dei tag del programma e Marketo gestisce automaticamente il resto.

**Modelli di pagina di destinazione/e-mail:** I modelli di pagina di destinazione/e-mail vengono importati in Design Studio. È possibile utilizzare le regole di conflitto per configurare il comportamento quando esiste un modello con lo stesso nome. Utilizzando la regola predefinita, a un modello viene aggiunto un numero se ne esiste già uno con lo stesso nome. Ad esempio, se disponi già di un modello denominato &quot;Modello standard&quot;, il nuovo sarà denominato &quot;Modello standard - 1&quot;.

**Pagine di destinazione/Forms:** Se in Design Studio esiste un modulo o una pagina di destinazione con lo stesso nome, verranno comunque importati, ma con un numero aggiunto al nome (ad esempio: Pagina di destinazione - 1).

**Immagini:** Le immagini utilizzate dalle pagine di destinazione vengono importate nello studio di progettazione a meno che non esista una con lo stesso nome.

**Token:** I token che risiedono al di fuori di un programma verranno convertiti in token locali durante il processo di importazione.

>[!CAUTION]
>
>I token di tipo immagine non sono supportati per le importazioni di programmi. Se viene importato un programma con un tipo di immagine i miei token, passeranno _no_ token.

**Tag programma:** È possibile utilizzare le regole di conflitto per controllare il modo in cui verranno trattati i tag programma che non esistono nell&#39;account di destinazione. L’utilizzo della regola predefinita creerà i tag del programma oppure puoi scegliere di ignorarli.

>[!CAUTION]
>
>Durante l&#39;importazione di un programma, le e-mail e le pagine di destinazione contenenti [contenuto dinamico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md){target="_blank"} verranno ignorate.
