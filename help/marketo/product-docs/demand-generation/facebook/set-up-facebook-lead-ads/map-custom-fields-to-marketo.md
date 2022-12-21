---
unique-page-id: 12983101
description: Mappatura di campi personalizzati su Marketo - Documenti Marketo - Documentazione del prodotto
title: Mappatura di campi personalizzati su Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Mappatura di campi personalizzati su Marketo {#map-custom-fields-to-marketo}

Per impostazione predefinita, è possibile raccogliere più informazioni rispetto alle informazioni standard memorizzate da Facebook, ad esempio la frequenza con cui un utente utilizza il servizio di consegna online. Puoi eseguire questa operazione tramite [creazione di domande personalizzate](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) nei tuoi annunci lead Facebook.

Tuttavia, **Marketo non inizierà automaticamente a raccogliere questi dati**. Per consentire a Marketo di iniziare a acquisire i valori dei campi personalizzati, è necessario **deve** mappare tali campi personalizzati su un campo in Marketo.

Ecco come configurarlo nell’area LaunchPoint di Admin.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai all&#39;area Amministratore e fai clic su **LaunchPoint**. In Servizi installati, trova e modifica **Annunci lead facebook**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Fai clic su **Successivo**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Lascia l&#39;account autorizzato così com&#39;è—do **not** apporta eventuali modifiche. Fai clic su **Successivo**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Come in precedenza, lascia le pagine selezionate così come sono. **not** apporta eventuali modifiche. Fai clic su **Successivo**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. Qui puoi mappare il campo Facebook personalizzato sul campo Marketo. Fai clic su **Aggiungi.**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. Nella nuova riga , immetti il nome del campo personalizzato Facebook .

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Solo i campi salvati nei modelli di modulo Facebook verranno visualizzati come opzioni.

1. Fai clic in **Campo Marketo** colonna. Digitare per cercare il campo a cui si desidera eseguire la mappatura. Dopo aver selezionato un campo, fai clic su **Salva**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Se non disponi già di un campo in Marketo su cui mappare il campo Facebook, scopri come [creare campi personalizzati](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>You **deve** segui questo processo per qualsiasi nuovo campo Facebook per consentire a Marketo di raccogliere i dati.
