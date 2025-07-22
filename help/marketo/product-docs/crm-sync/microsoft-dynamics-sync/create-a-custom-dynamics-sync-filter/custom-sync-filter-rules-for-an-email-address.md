---
unique-page-id: 10095307
description: Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail {#custom-sync-filter-rules-for-an-email-address}

Per evitare la sincronizzazione di record privi di indirizzo e-mail, attieniti a queste regole.

* Quando viene creato un lead OPPURE quando il campo dell&#39;indirizzo e-mail del lead viene aggiornato, verificare che il lead disponga di un indirizzo e-mail e, in caso affermativo, modificare Sync in Mkto in **[!UICONTROL True]**. Altrimenti cambia in **[!UICONTROL False]**

* Quando viene creato un contatto O quando il campo dell&#39;indirizzo e-mail del contatto viene aggiornato, verificare se il contatto dispone di un indirizzo e-mail e, in caso affermativo, modificare Sync in Mkto in **[!UICONTROL True]** e cambiare Sync in Mkto in **[!UICONTROL True]** nel record Account. In caso contrario, modifica in **[!UICONTROL False]**

* Quando il campo Nome società del contatto (parentcustomerid) viene aggiornato, verifica se il campo Sync to Mkto del contatto è true. In caso affermativo, impostare Sync su Mkto sull&#39;account su **[!UICONTROL True]**
* Quando viene aggiornato il campo del potenziale cliente dell’opportunità (customerid) o del contatto (parentcontactid), verifica se il campo Sync to Mkto dell’account è true o se il campo Sync to Mkto del contatto è true. In caso affermativo, modificare Sync in Mkto sull&#39;opportunità in **[!UICONTROL True]** anche
