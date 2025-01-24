---
title: Utilizzare Experience Manager Assets
description: Scopri come utilizzare le risorse di immagini da un archivio AEM Assets connesso durante l’authoring dei contenuti in Adobe Marketo Engage.
hide: true
hidefromtoc: true
source-git-commit: c6132bf5b393df38700ad9dd6f0c6414860e8bb6
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 1%

---

# Utilizzare risorse Experience Manager

Quando Adobe Experience Manager Assets as a Cloud Service è integrato con Adobe Marketo Engage, puoi individuare e accedere facilmente alle risorse digitali da utilizzare nei contenuti di marketing. Quando crei i contenuti, le risorse sono accessibili dall&#39;elemento _[!UICONTROL Assets]_ nell&#39;area di navigazione a sinistra e quando crei contenuti e-mail per un percorso di account. Puoi anche caricare le risorse nell’archivio as a Cloud Service di AEM Assets connesso direttamente da Adobe Journey Optimizer B2B edition.

>[!NOTE]
>
>Al momento, in Adobe Journey Optimizer B2B edition sono supportate solo le risorse immagine di Adobe Experience Manager Assets. Le modifiche alle risorse devono essere effettuate dall’archivio centrale di Adobe Experience Manager Assets. [Ulteriori informazioni](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/manage-digital-assets)

Quando utilizzi queste risorse digitali, le modifiche più recenti apportate in Assets as a Cloud Service si propagano automaticamente alle campagne e-mail live tramite riferimenti collegati. Se le immagini vengono eliminate in Adobe Experience Manager Assets as a Cloud Service, nelle e-mail vengono visualizzate con un riferimento non funzionante. Quando le risorse attualmente utilizzate nei percorsi di account vengono modificate o eliminate, gli autori del percorso ricevono una notifica sulle modifiche apportate all’immagine e sull’elenco dei percorsi che la utilizzano. Tutte le modifiche apportate alle risorse devono essere effettuate nell’archivio centrale di Adobe Experience Manager Assets.

## Utilizza AEM Assets come origine dell’immagine

Se il tuo ambiente dispone di una o più connessioni a archivi Assets, puoi designare AEM Assets come origine per le risorse quando crei o visualizzi i dettagli di un’e-mail, un modello e-mail o un frammento visivo.

* Quando crei un nuovo contenuto, scegli `AEM Assets` come elemento **[!UICONTROL Image Source]** nella finestra di dialogo.

SCHERMATA

* Quando apri una risorsa di contenuto esistente, scegli `AEM Assets` nel pannello _[!UICONTROL Corpo]_ a destra.

SCHERMATA

## Accedere alle risorse per la creazione

>[!IMPORTANT]
>
>Un amministratore deve aggiungere gli utenti che hanno bisogno di accedere ad Assets ai profili di prodotto Utenti consumer di Assets e Utenti di Assets. [Ulteriori informazioni](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/security/ims-support#managing-products-and-user-access-in-admin-console)

Nell&#39;editor di contenuti visivi, fai clic sull&#39;icona _Selettore risorse_ nella barra laterale a sinistra. In questo modo il pannello strumenti diventa un elenco delle risorse disponibili nell’archivio selezionato.

SCHERMATA

Se sono presenti più repository AEM connessi, fare clic sulla freccia del menu relativa a **[!UICONTROL Repository]** per scegliere il repository che si desidera utilizzare.

SCHERMATA

Esistono diversi metodi per aggiungere una risorsa immagine all’area di lavoro visiva:

* Trascina e rilascia la miniatura di un’immagine dal menu di navigazione a sinistra.

SCHERMATA

* Aggiungi un componente immagine all&#39;area di lavoro e fai clic su **[!UICONTROL Sfoglia]** per aprire la finestra di dialogo _[!UICONTROL Seleziona Assets]_.

  Dalla finestra di dialogo, puoi scegliere un’immagine dall’archivio selezionato.

  Sono disponibili diversi strumenti per aiutarti a individuare la risorsa di cui hai bisogno.

SCHERMATA

* Modifica l&#39;**[!UICONTROL Archivio]** in alto a destra.

* Fai clic su **[!UICONTROL Gestisci risorse]** in alto a destra per aprire l&#39;archivio Assets in un&#39;altra scheda del browser e utilizzare gli strumenti di gestione AEM Assets.

* Fai clic sul selettore _Tipo di visualizzazione_ in alto a destra per modificare la visualizzazione in **[!UICONTROL Vista a elenco]**, **[!UICONTROL Vista griglia]**, **[!UICONTROL Vista galleria]** o **[!UICONTROL Vista a cascata]**.

* Fai clic sull&#39;icona _Ordinamento_ per modificare l&#39;ordinamento tra crescente e decrescente.

* Fare clic sulla freccia del menu **[!UICONTROL Ordina per]** per modificare i criteri di ordinamento in **[!UICONTROL Nome]**, **[!UICONTROL Dimensione]** o **[!UICONTROL Modificato]**.

* Fai clic sull&#39;icona _Filtro_ in alto a sinistra per filtrare gli elementi visualizzati in base ai criteri.

* Immetti il testo da cercare nel campo Ricerca per filtrare gli elementi visualizzati in modo che corrispondano al nome della risorsa.

SCHERMATA
