---
unique-page-id: 14352592
description: Scopri come inserire campi dinamici nei modelli di Sales Connect. Aggiungi nome, società e altri campi unione nell’editor modelli.
title: Come inserire campi dinamici
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/WwKaorfXBu5Ah9wD6pXf5U4YzlpP9MoUMg-TtDzXDRo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 239
ht-degree: 4%

---

# Come inserire campi dinamici {#how-to-insert-dynamic-fields}

È possibile personalizzare i modelli e-mail con attributi predefiniti come `{{first_name}}` o `{{company}}`. Questi campi ti consentono di inviare tramite e-mail più contatti e di completarli automaticamente senza doverli digitare separatamente per ciascun contatto.

>[!TIP]
>
>Il campo &quot;first_name&quot; e &quot;company&quot; sono gli unici campi che verranno cercati sia in [!DNL Sales Connect] che in [!DNL Salesforce]. Ciò significa che se un contatto non esiste nell&#39;applicazione Web [&#128279;](https://toutapp.com/login), verrà eseguita una ricerca in [!DNL Salesforce] per verificare se è possibile trovare un record contatto/lead con un indirizzo e-mail corrispondente. Quindi utilizziamo le informazioni di quel record per compilare il campo.

## Inserire un campo dinamico in un modello {#insert-a-dynamic-field-into-a-template}

1. In **[!UICONTROL Templates & Campaigns]**, trovare il modello da modificare e fare clic su **[!UICONTROL Edit Template]**.

1. Fai clic su **[!UICONTROL Tout Dynamic Fields]**.

   >[!NOTE]
   >
   >Quando si inviano messaggi di posta elettronica a contatti esistenti in [!DNL Sales Connect], è possibile utilizzare i campi dinamici di base. Questi richiameranno direttamente dal contatto.

Se si inviano messaggi di posta elettronica a contatti esistenti in [!DNL Salesforce], è possibile sfruttare i campi dinamici [!DNL Salesforce]. Questi iniziano tutti con &quot;sfdc&quot;. Se si dispone di una connessione a [!DNL Salesforce], questi campi chiameranno direttamente il lead/contatto in [!DNL Salesforce] per compilare le informazioni nel modello.

## Inserire campi dinamici in un oggetto {#insert-dynamic-fields-in-a-subject-line}

È sufficiente copiarli e incollarli manualmente nel campo dell’oggetto di un’e-mail, assicurandosi di disporre della formattazione corretta.
