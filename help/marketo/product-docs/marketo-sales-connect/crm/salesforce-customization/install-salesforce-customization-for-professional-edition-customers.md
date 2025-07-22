---
unique-page-id: 27656223
description: Installa [!DNL Salesforce] Personalizzazione per clienti Professional Edition - Documentazione di Marketo - Documentazione del prodotto
title: Installa [!DNL Salesforce] Personalizzazione per i clienti Professional Edition
exl-id: dc004a28-b580-4449-9fde-e744681ac53a
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Installa la personalizzazione [!DNL Salesforce] per i clienti Professional Edition {#install-salesforce-customization-for-professional-edition-customers}

I clienti con [!DNL Salesforce] Professional Edition dovranno seguire questi passaggi per installare la personalizzazione.

>[!PREREQUISITES]
>
>* L&#39;amministratore [!DNL Sales Connect] deve connettere i propri account [!DNL Salesforce] e [!DNL Sales Connect].
>* L&#39;istanza [!DNL Salesforce] utilizzata deve disporre di spazio per installare tredici campi attività personalizzati.

## Installazione {#installation}

1. In [!DNL Sales Connect], fare clic sull&#39;icona ingranaggio in alto a destra e selezionare **[!UICONTROL Settings]**.

   ![](assets/one-4.png)

1. In [!UICONTROL Admin Settings], fare clic su **[!UICONTROL Salesforce]**.

   ![](assets/two-4.png)

1. Verificare di essere connessi all&#39;account [!DNL Salesforce].

   >[!CAUTION]
   >
   >Se si è connessi, verrà visualizzato un pulsante verde &quot;[!UICONTROL Install]&quot;. **DO NOT** fare clic su questo pulsante, passare al passaggio 4.

1. Accedi all&#39;account [!DNL Salesforce] a cui sei connesso e quindi fai clic su [questo collegamento](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t0b000001oWEZ).
1. Verrà visualizzata la pagina di installazione di [!DNL Sales Connect].

   ![](assets/install-package.png)

1. Scegli gli utenti per i quali desideri installare le personalizzazioni: solo amministratore, tutti gli utenti o profili specifici.
1. Fare clic sul pulsante **[!UICONTROL Install]** per installare la personalizzazione.
1. Per confermare l&#39;installazione, accedere al proprio account [!DNL Salesforce].
1. Fare clic su **[!UICONTROL Setup]**, cercare &quot;Pacchetti installati&quot; nella barra di ricerca e fare clic su **[!UICONTROL Installed Packages]**.

   Qui verranno visualizzate le personalizzazioni di Marketo Sales Connect.

   Per configurare [!DNL Sales Connect] nell&#39;istanza di [!DNL Salesforce], seguire i passaggi a partire dalla sezione &quot;CONFIGURAZIONE DEL PACCHETTO SALES ENGAGE SALESFORCE&quot; a pagina 7 della Guida all&#39;installazione.

   >[!NOTE]
   >
   >[!DNL Sales Engage] è il nome precedente per [!DNL Sales Connect].

## Guide {#guides}

[Guida all&#39;installazione per Salesforce Classic](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)

[Guida all&#39;installazione per Salesforce Lightning](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
