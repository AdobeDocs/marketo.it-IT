---
unique-page-id: 12983101
description: Mappatura di campi personalizzati su Marketo - Documentazione Marketo - Documentazione del prodotto
title: Mappa campi personalizzati su Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Mappa campi personalizzati su Marketo {#map-custom-fields-to-marketo}

Per impostazione predefinita, potrebbe essere utile raccogliere più informazioni rispetto a quelle standard memorizzate da Facebook, ad esempio la frequenza con cui un utente utilizza il servizio di consegna online. Puoi eseguire questa operazione [creando domande personalizzate](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) nei tuoi annunci lead di Facebook.

Tuttavia, **Marketo non inizierà automaticamente a raccogliere questi dati**. Affinché Marketo possa iniziare a catturare i valori dei campi personalizzati, **devi** mappare tali campi personalizzati a un campo in Marketo.

Per effettuare questa configurazione, consulta l’area LaunchPoint in Amministrazione.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai all&#39;area di amministrazione e fai clic su **LaunchPoint**. In Servizi installati, trovare e modificare **Annunci lead Facebook**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Fai clic su **Avanti**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Lascia invariato l&#39;account autorizzato. **non** apportare modifiche. Fai clic su **Avanti**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Come prima, lascia invariate le pagine selezionate—fai **no** per apportare modifiche. Fai clic su **Avanti**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. Il campo Facebook personalizzato viene mappato sul campo Marketo. Fare clic su **Aggiungi.**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. Nella nuova riga, immetti il nome del campo personalizzato Facebook.

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Solo i campi salvati nei modelli di modulo di Facebook verranno visualizzati come opzioni qui.

1. Fare clic nella colonna **Campo Marketo**. Digitare per cercare il campo a cui si desidera eseguire il mapping. Dopo aver selezionato un campo, fai clic su **Salva**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Se non disponi già di un campo in Marketo a cui mappare il campo Facebook, scopri come [creare campi personalizzati](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>Per consentire a Marketo di raccogliere i dati, **devi** eseguire questa procedura per qualsiasi nuovo campo Facebook.
