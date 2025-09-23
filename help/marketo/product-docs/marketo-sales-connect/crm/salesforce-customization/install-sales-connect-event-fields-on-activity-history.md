---
unique-page-id: 14352475
description: Installare i campi evento Sales Connect nella cronologia attività - Documentazione Marketo - Documentazione del prodotto
title: Installare campi evento Sales Connect nella cronologia attività
exl-id: c1bdb5a6-04f0-4579-84b6-33f4a301128f
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 9%

---

# Installare campi evento Sales Connect nella cronologia attività {#install-sales-connect-event-fields-on-activity-history}

Dopo aver installato il pacchetto Enterprise in [!DNL Salesforce], puoi installare [!UICONTROL Sales Connect] campi evento nella sezione della cronologia attività. I campi dell&#39;evento [!UICONTROL Sales Connect] includono informazioni quali visualizzazioni, clic e campagne. Ciò ti consente di importare direttamente in [!DNL Salesforce] le informazioni sulle e-mail.

Assicurati di aver contattato l&#39;amministratore [!DNL Salesforce] durante l&#39;esecuzione di questi passaggi. In questo esempio i campi verranno installati nel **Layout pagina lead**. È inoltre possibile installare i campi nei layout di pagina Contatto, Account e Opportunità. Ricorda che quando si registrano le e-mail su account e opportunità è necessario il contatto a cui si sta inviando l’e-mail come ruolo di contatto.

1. Fai clic su **[!UICONTROL Setup]**.
1. Fai clic su **[!UICONTROL Customize]**.
1. Fai clic su **[!UICONTROL Leads]**.
1. Fai clic su **[!UICONTROL Page Layouts]**.
1. Fare clic su **[!UICONTROL Edit]** accanto al layout di pagina che si desidera modificare.

   >[!NOTE]
   >
   >[!DNL Sales Connect] installerà alcuni layout di pagina, ma se ne hai già uno predefinito che il tuo team sta utilizzando dovrai installarlo lì. È possibile eliminare i layout di pagina [!DNL Sales Connect] se non si desidera utilizzarli.

1. Scorri verso il basso fino alla sezione [!UICONTROL Activity History].
1. Fai clic sulla chiave inglese da modificare.
1. Selezionare i campi [!UICONTROL Sales Connect] da includere nella sezione [!UICONTROL Activity History]. Se non trovi [!UICONTROL Sales Connect] campi qui, potresti aver installato il pacchetto [!DNL Salesforce] errato.
1. Fare clic su **[!UICONTROL Add]** per spostare i campi desiderati.
1. Fai clic su **[!UICONTROL OK]**.
1. Fai clic su **[!UICONTROL Save]**.

   Gli utenti potranno ora visualizzare informazioni e aggiornamenti utili sulle e-mail in [!DNL Salesforce].
