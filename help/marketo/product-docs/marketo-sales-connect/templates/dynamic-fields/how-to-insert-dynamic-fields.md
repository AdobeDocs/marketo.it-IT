---
unique-page-id: 14352592
description: Come inserire campi dinamici - Documentazione di Marketo - Documentazione del prodotto
title: Come inserire campi dinamici
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '222'
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

Se invii messaggi di posta elettronica a contatti esistenti in [!DNL Salesforce], puoi sfruttare i campi dinamici [!DNL Salesforce]. Questi iniziano tutti con &quot;sfdc&quot;. Se si dispone di una connessione a [!DNL Salesforce], questi campi chiameranno direttamente il lead/contatto in [!DNL Salesforce] per compilare le informazioni nel modello.

## Inserire campi dinamici in un oggetto {#insert-dynamic-fields-in-a-subject-line}

È sufficiente copiarli e incollarli manualmente nel campo dell’oggetto di un’e-mail, assicurandosi di disporre della formattazione corretta.
