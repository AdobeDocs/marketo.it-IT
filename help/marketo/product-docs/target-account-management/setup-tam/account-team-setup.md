---
unique-page-id: 11384433
description: Scopri come impostare i team dell’account e mappare i ruoli dell’account CRM su TAM. Scegliere i campi di ricerca utente che diventeranno membri del team account.
title: Configurazione team account
exl-id: a4aee37f-5e39-4296-b720-b1c73c98df9e
feature: Target Account Management
TQID: 'https://experienceleague.adobe.com/UyREfPyH-7ICes5S0VhIcu-3MsS5TlNG40TcZ9z5w94'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
subfeature_v2:
  - id: fd4ca7b1-bd80-47f4-ad1a-846912e45cc5
    internal-label: Target Account Management
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 5%
---
# Configurazione team account {#account-team-setup}

Un team di account è un gruppo di stakeholder che lavorano insieme su un account con nome. Segui questi passaggi per scegliere quali ruoli dell’account CRM aggiungere.

1. Fai clic su **[!UICONTROL Admin]**.

   ![](assets/one-3.png)

1. Fai clic su **[!UICONTROL Target Account Management]**.

   ![](assets/account-team-setup-2.png)

1. In Membri team account fare clic su **[!UICONTROL Edit]**.

   ![](assets/3.png)

   >[!NOTE]
   >
   >Per [!UICONTROL Account Role], assegnargli un nome e confrontarlo con il campo di ricerca utente desiderato nel CRM.

1. Digita il tuo nome [!UICONTROL Account Role] e seleziona il campo **CRM**. Somma fino a 10.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >Impossibile selezionare [!UICONTROL Account Owner]. Viene scelto per impostazione predefinita dal livello account nel CRM.

1. Al termine, fai clic su **[!UICONTROL Save]**.

   ![](assets/five-2.png)

   >[!CAUTION]
   >
   >Se effettui un aggiornamento, la visualizzazione delle modifiche in TAM potrebbe impiegare del tempo.

   >[!NOTE]
   >
   >* Quando più account CRM con proprietari account diversi vengono uniti in un account denominato, Marketo sceglierà un &quot;Proprietario account&quot; e aggiungerà altri proprietari account come &quot;Proprietari account&quot;
   >
   >* Se un campo &quot;Ruolo&quot; del CRM viene successivamente rinominato o eliminato, Marketo TAM interromperà la sincronizzazione dei valori aggiornati fino a quando l’utente non aggiorna manualmente la configurazione in TAM
