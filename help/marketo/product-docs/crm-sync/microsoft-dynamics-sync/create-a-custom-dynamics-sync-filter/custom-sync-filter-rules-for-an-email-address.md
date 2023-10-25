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

* Quando viene creato un lead OPPURE quando il campo dell’indirizzo e-mail del lead viene aggiornato, verifica se il lead ha un indirizzo e-mail e, in caso affermativo, modifica Sincronizza con Mkto in **[!UICONTROL Vero]**. Altrimenti modifica in **[!UICONTROL Falso]**.

* Quando viene creato un contatto O quando il campo dell’indirizzo e-mail del contatto viene aggiornato, verifica se il contatto dispone di un indirizzo e-mail e, in caso affermativo, modifica Sincronizza con Mkto in **[!UICONTROL Vero]** e cambia da Sincronizza a Mkto a **[!UICONTROL Vero]** nel record Account. In caso contrario, modifica in **[!UICONTROL Falso]**.

* Quando il campo Nome società del contatto (parentcustomerid) viene aggiornato, verificare se il campo Sincronizza con Mkto del contatto è impostato su true. In caso affermativo, impostare Sincronizza su Mkto sull&#39;account in **[!UICONTROL Vero]** anche.

* Quando il campo Potenziale cliente (customerid) dell’opportunità o Contatto (parentcontactid) viene aggiornato, verifica se il campo Sincronizza con Mkto dell’account è true o se il campo Sincronizza con Mkto del contatto è true. In caso affermativo, modifica Sync in Mkto sull’opportunità in **[!UICONTROL Vero]** anche.
