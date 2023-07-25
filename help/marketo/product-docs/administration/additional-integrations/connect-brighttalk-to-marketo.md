---
unique-page-id: 15695874
description: "Connetti [!DNL BrightTALK] alla documentazione Marketo - Marketo - Documentazione del prodotto"
title: "Connetti [!DNL BrightTALK] a Marketo"
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
feature: Administration, Integrations
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 1%

---

# Connetti [!DNL BrightTALK] a MARKETO {#connect-brighttalk-to-marketo}

Scopri come collegare il tuo [!DNL BrightTALK] alla tua istanza Marketo. A questo scopo, devi essere un amministratore per entrambi.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Passaggi [!DNL BrightTALK] {#steps-in-brighttalk}

1. Accedi a [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target="_blank"} e fai clic su **[!UICONTROL Connetti]**.
1. Sotto [!UICONTROL Connettore Marketo avanzato], fai clic su **[!UICONTROL Connetti]**.
1. Viene visualizzata la schermata delle credenziali in cui vengono richiesti: ID client, Segreto client, URL del servizio identità e URL del servizio rest. Per ottenere queste informazioni, accedi a Marketo.

## Passaggi in Marketo {#steps-in-marketo}

>[!NOTE]
>
>A questo punto ti verrà richiesto di impostare un [!DNL API Only User Role] e [!DNL API User] per limitare le autorizzazioni [!DNL BrightTALK] avrà nell’istanza di Marketo. Poiché disponiamo già di articoli per questi passaggi, ti collegheremo a essi.

1. Creare un [Solo ruolo utente API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}.

1. [Creare un utente API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"}, utilizzando [!DNL BrightTALK] Ruolo API creato durante il passaggio 4.

1. Torna a **[!UICONTROL Amministratore]** area.

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. Sotto **[!UICONTROL Integrazione]**, fai clic su **[!UICONTROL LaunchPoint]**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. Fai clic su **[!UICONTROL Nuovo]** a discesa e selezionare **[!UICONTROL Nuovo servizio]**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. Immetti un **[!UICONTROL Nome visualizzato]** di tua scelta. Fai clic su **[!UICONTROL Servizio]** a discesa e selezionare **[!UICONTROL Personalizzato]** (fare _non_ seleziona [!DNL BrightTALK]).

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >Ricordati di non selezionare [!DNL BrightTALK] nel menu a discesa. Si tratta di un campo che stiamo rimuovendo e la sua selezione potrebbe creare problemi significativi con il tuo [!DNL Marketo/BrightTALK] integrazione.

1. Immetti un [!UICONTROL Descrizione] di tua scelta. Fai clic su **[!UICONTROL Utente solo API]** e selezionare il [!DNL BrightTALK API User] creato durante il passaggio 5. Fai clic su **[!UICONTROL Crea]**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. Clic **[!UICONTROL Visualizza dettagli]** per il servizio personalizzato appena creato.

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. Copia (e salva) il **[!UICONTROL ID client]** e **[!UICONTROL Segreto client]**. Fai clic su **[!UICONTROL Chiudi]**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. Sotto **[!UICONTROL Integrazione]**, seleziona **[!UICONTROL Servizi Web]**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. Sotto **[!UICONTROL API REST]**, copia (e salva) il **[!UICONTROL Endpoint]** e **[!UICONTROL Identità]**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## Passaggi aggiuntivi in [!DNL BrightTALK] {#additional-steps-in-brighttalk}

1. Torna a [!DNL BrightTALK] schermata di configurazione del connettore dal passaggio 3 e immettere le credenziali salvate dai passaggi 12 e 14.

Dopo l&#39;autenticazione delle credenziali, è stata stabilita la connessione ufficiale [!DNL BrightTALK] a Marketo. Il passaggio successivo consiste nel determinare [quali campi dati si desidera sincronizzare](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target="_blank"}.
