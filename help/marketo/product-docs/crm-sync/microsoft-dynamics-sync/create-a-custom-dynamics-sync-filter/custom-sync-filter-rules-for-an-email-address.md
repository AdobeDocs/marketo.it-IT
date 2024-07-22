---
unique-page-id: 10095307
description: Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail {#custom-sync-filter-rules-for-an-email-address}

Per evitare la sincronizzazione di record privi di indirizzo e-mail, attieniti a queste regole.

* Quando viene creato un lead OPPURE quando il campo dell&#39;indirizzo e-mail del lead viene aggiornato, verificare se il lead ha un indirizzo e-mail e, in caso affermativo, impostare Sync su Mkto su **[!UICONTROL True]**. In caso contrario, impostare su **[!UICONTROL False]**.

* Quando viene creato un contatto OPPURE quando il campo dell&#39;indirizzo di posta elettronica del contatto viene aggiornato, verificare se il contatto dispone di un indirizzo di posta elettronica e, in caso affermativo, impostare Sync su Mkto su **[!UICONTROL True]** e impostare Sync su Mkto su **[!UICONTROL True]** nel record Account. In caso contrario, impostare su **[!UICONTROL False]**.

* Quando il campo Nome società del contatto (parentcustomerid) viene aggiornato, verificare se il campo Sincronizza con Mkto del contatto è impostato su true. In caso affermativo, impostare Sincronizza su Mkto sull&#39;account su **[!UICONTROL True]**.

* Quando il campo Potenziale cliente (customerid) dell’opportunità o Contatto (parentcontactid) viene aggiornato, verifica se il campo Sincronizza con Mkto dell’account è true o se il campo Sincronizza con Mkto del contatto è true. In caso affermativo, impostare Sincronizza su Mkto anche per l&#39;opportunità su **[!UICONTROL True]**.
