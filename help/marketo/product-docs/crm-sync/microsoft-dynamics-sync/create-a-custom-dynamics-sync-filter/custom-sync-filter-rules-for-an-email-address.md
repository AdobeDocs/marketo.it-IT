---
unique-page-id: 10095307
description: Scopri come impostare regole di filtro di sincronizzazione personalizzate per l’indirizzo e-mail in Dynamics. Utilizza i flussi di lavoro per impostare la sincronizzazione su Mkto in base al fatto che il lead o il contatto abbia un’e-mail.
title: Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 7%

---

# Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail {#custom-sync-filter-rules-for-an-email-address}

Per evitare la sincronizzazione di record privi di indirizzo e-mail, attieniti a queste regole.

* Quando viene creato un lead OPPURE quando il campo dell&#39;indirizzo e-mail del lead viene aggiornato, verificare che il lead disponga di un indirizzo e-mail e, in caso affermativo, modificare Sync in Mkto in **[!UICONTROL True]**. Altrimenti cambia in **[!UICONTROL False]**

* Quando viene creato un contatto O quando il campo dell&#39;indirizzo e-mail del contatto viene aggiornato, verificare se il contatto dispone di un indirizzo e-mail e, in caso affermativo, modificare Sync in Mkto in **[!UICONTROL True]** e cambiare Sync in Mkto in **[!UICONTROL True]** nel record Account. In caso contrario, modifica in **[!UICONTROL False]**

* Quando il campo Nome società del contatto (parentcustomerid) viene aggiornato, verifica se il campo Sync to Mkto del contatto è true. In caso affermativo, impostare Sync su Mkto sull&#39;account su **[!UICONTROL True]**
* Quando viene aggiornato il campo del potenziale cliente dell’opportunità (customerid) o del contatto (parentcontactid), verifica se il campo Sync to Mkto dell’account è true o se il campo Sync to Mkto del contatto è true. In caso affermativo, modificare Sync in Mkto sull&#39;opportunità in **[!UICONTROL True]** anche
