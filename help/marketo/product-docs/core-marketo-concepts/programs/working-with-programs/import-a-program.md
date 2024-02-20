---
unique-page-id: 1147108
description: Importare un programma - Documentazione di Marketo - Documentazione del prodotto
title: Importare un programma
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
feature: Programs
source-git-commit: 0adb780ea1622d12b8daafc502fd6a9151757ad3
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Importare un programma {#import-a-program}

Un programma può essere importato da un abbonamento di Marketo Engage a un altro. Ad esempio, puoi creare un programma in una sandbox e quindi importarlo nel tuo abbonamento live. Inoltre, puoi importare un programma predefinito da [Libreria programmi Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/program-library/program-import-library-overview.md){target="_blank"}.

>[!CAUTION]
>
>I programmi che dispongono di elenchi avanzati contenenti un trigger &quot;L’oggetto personalizzato è aggiornato&quot; causeranno l’interruzione dell’importazione. Rimuovi questo trigger da tutti gli elenchi smart prima di seguire i passaggi descritti di seguito.

## Importazione di un programma {#importing-a-program}

1. Vai a **[!UICONTROL Attività di marketing]**.

   ![](assets/import-a-program-1.png)

1. Fai clic su **[!UICONTROL Nuovo]** a discesa e selezionare **[!UICONTROL Importa programma]**.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >* Importazione programmi è disponibile solo per gli utenti che dispongono di ruoli con l&#39;autorizzazione Importazione programmi abilitata. Ulteriori informazioni su [gestione di ruoli utente e autorizzazioni](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.
   >
   >* Per collegare un account sandbox al tuo abbonamento live, contatta [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. Seleziona un Marketo **[!UICONTROL Abbonamento]** e un programma da importare. Clic **[!UICONTROL Successivo]**.

   ![](assets/import-a-program-3.png)

1. Specifica un **[!UICONTROL Cartella campagna]** per il programma importato. Clic **[!UICONTROL Successivo]**.

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >Assicurati che **[!UICONTROL Usa conflitto predefinito]** regole è selezionato. Le regole di conflitto sono necessarie quando si importano programmi in un&#39;istanza con risorse con lo stesso nome.

1. Scegli i dettagli del conflitto desiderati e fai clic su **[!UICONTROL Successivo]**.

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >Quando si importa un programma che utilizza i passaggi di flusso personalizzati o le regole di elenchi avanzati derivate da un servizio di passaggi di flusso in un&#39;istanza di destinazione in cui è presente più di un provider di servizi compatibile, all&#39;utente di importazione viene richiesto di assegnare i passaggi o le regole al provider di servizi corretto nell&#39;istanza di destinazione.

1. Dettagli anteprima e **[!UICONTROL Importa]** il programma.

   ![](assets/import-a-program-6.png)

Al termine dell’importazione riceverai una conferma e-mail.

>[!NOTE]
>
>Dovrai riprogrammare le campagne batch importate e attivare le campagne trigger. Il sistema disattiva automaticamente le pianificazioni delle campagne e attiva le campagne nel programma importato.

## Impatto sulle risorse esterne durante le importazioni del programma {#impact-on-external-assets-during-program-imports}

I programmi utilizzano risorse esterne come modelli e-mail, modelli di pagina di destinazione, immagini, moduli, token e tag di programma. È possibile configurare la modalità di gestione dei modelli della pagina di destinazione e dei tag del programma e Marketo gestisce automaticamente il resto.

**Modelli di pagina di destinazione/e-mail:** I modelli di e-mail/pagina di destinazione vengono importati in Design Studio. È possibile utilizzare le regole di conflitto per configurare il comportamento quando esiste un modello con lo stesso nome. Utilizzando la regola predefinita, a un modello viene aggiunto un numero se ne esiste già uno con lo stesso nome. Ad esempio, se disponi già di un modello denominato &quot;Modello standard&quot;, il nuovo sarà denominato &quot;Modello standard - 1&quot;.

**Pagine di destinazione/Forms:** Se in Design Studio esiste un modulo o una pagina di destinazione con lo stesso nome, questi verranno comunque importati, ma con un numero aggiunto al nome (ad esempio, Pagina di destinazione - 1).

**Immagini:** Le immagini utilizzate dalle pagine di destinazione vengono importate nello studio di progettazione a meno che non esista un&#39;immagine con lo stesso nome.

**Token:** I token che risiedono al di fuori di un programma verranno convertiti in token locali durante il processo di importazione.

>[!CAUTION]
>
>I token di tipo immagine non sono supportati per le importazioni di programmi. Se viene importato un programma con tipo di immagine i miei token, _no_ i token passeranno attraverso.

**Tag programma:** Puoi utilizzare le regole di conflitto per controllare il modo in cui verranno trattati i tag del programma che non esistono nell’account di destinazione. L’utilizzo della regola predefinita creerà i tag del programma oppure puoi scegliere di ignorarli.

>[!CAUTION]
>
>Durante l’importazione di un programma, e-mail/pagine di destinazione contenenti [contenuto dinamico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md){target="_blank"} verrà ignorato.
