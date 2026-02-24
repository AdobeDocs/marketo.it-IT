---
unique-page-id: 15695874
description: Connetti [!DNL BrightTALK] a Marketo - Documentazione Marketo - Documentazione del prodotto
title: Connetti [!DNL BrightTALK] a Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
feature: Administration, Integrations
source-git-commit: 7f8968210659ed2c51640966115f22da47e42ebf
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 3%

---

# Connetti [!DNL BrightTALK] a Marketo {#connect-brighttalk-to-marketo}

Scopri come collegare il canale [!DNL BrightTALK] all&#39;istanza Marketo. A questo scopo, devi essere un amministratore per entrambi.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Passaggi in [!DNL BrightTALK] {#steps-in-brighttalk}

1. Accedi a [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target="_blank"} e fai clic su **[!UICONTROL Connect Now]**.
1. In [!UICONTROL Advanced Marketo Connector], fare clic su **[!UICONTROL Connect]**.
1. Viene visualizzata la schermata delle credenziali in cui vengono richiesti: ID client, Segreto client, URL del servizio identità e URL del servizio rest. Per ottenere queste informazioni, accedi a Marketo.

## Passaggi in Marketo {#steps-in-marketo}

>[!NOTE]
>
>A questo punto ti verrà richiesto di impostare [!DNL API Only User Role] e [!DNL API User] per limitare le autorizzazioni di [!DNL BrightTALK] nell&#39;istanza di Marketo. Poiché disponiamo già di articoli per questi passaggi, ti collegheremo a essi.

1. Crea un ruolo utente [solo API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}.

1. [Crea un utente API](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md){target="_blank"}, utilizzando il ruolo API [!DNL BrightTALK] creato durante il passaggio 4.

1. Torna all&#39;area **[!UICONTROL Admin]**.

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. In **[!UICONTROL Integration]**, fare clic su **[!UICONTROL LaunchPoint]**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. Fai clic sul menu a discesa **[!UICONTROL New]** e seleziona **[!UICONTROL New Service]**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. Immetti un **[!UICONTROL Display Name]** a tua scelta. Fai clic sul menu a discesa **[!UICONTROL Service]** e seleziona **[!UICONTROL Custom]** (fai _no_ seleziona [!DNL BrightTALK]).

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >Ricordarsi di non selezionare [!DNL BrightTALK] nel menu a discesa. È un campo che stiamo rimuovendo e la sua selezione potrebbe creare problemi significativi con l&#39;integrazione di [!DNL Marketo/BrightTALK].

1. Immetti un [!UICONTROL Description] a tua scelta. Fare clic sul menu a discesa **[!UICONTROL API Only User]** e selezionare [!DNL BrightTALK API User] creato durante il passaggio 5. Fai clic su **[!UICONTROL Create]**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. Fare clic su **[!UICONTROL View Details]** per il servizio personalizzato appena creato.

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. Copiare (e salvare) **[!UICONTROL Client ID]** e **[!UICONTROL Client Secret]**. Fai clic su **[!UICONTROL Close]**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. In **[!UICONTROL Integration]**, selezionare **[!UICONTROL Web Services]**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. In **[!UICONTROL Rest API]**, copiare (e salvare) **[!UICONTROL Endpoint]** e **[!UICONTROL Identity]**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## Passaggi aggiuntivi in [!DNL BrightTALK] {#additional-steps-in-brighttalk}

1. Tornare alla schermata di configurazione del connettore [!DNL BrightTALK] dal passaggio 3 e immettere le credenziali salvate dai passaggi 12 e 14.

Dopo l&#39;autenticazione delle credenziali, [!DNL BrightTALK] è stato ufficialmente connesso a Marketo. Il passaggio successivo consiste nel determinare quali campi dati si desidera sincronizzare. Se hai bisogno di assistenza, contatta il supporto all&#39;indirizzo [BrightTALK](https://www.brighttalk.com/){target="_blank"}.
