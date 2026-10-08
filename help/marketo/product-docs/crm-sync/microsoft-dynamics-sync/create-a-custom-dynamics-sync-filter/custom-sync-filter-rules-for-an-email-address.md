---
unique-page-id: 10095307
description: Scopri come impostare regole di filtro di sincronizzazione personalizzate per l’indirizzo e-mail in Dynamics. Utilizza i flussi di lavoro per impostare la sincronizzazione su Mkto in base al fatto che il lead o il contatto abbia un’e-mail.
title: Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/SPEV9J4rabu7tMrPEOW8JYg2r7ihtTzE6OmJZvkOIZ4'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 7%
---
# Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail {#custom-sync-filter-rules-for-an-email-address}

Per evitare la sincronizzazione di record privi di indirizzo e-mail, attieniti a queste regole.

* Quando viene creato un lead OPPURE quando il campo dell&#39;indirizzo e-mail del lead viene aggiornato, verificare che il lead disponga di un indirizzo e-mail e, in caso affermativo, modificare Sync in Mkto in **[!UICONTROL True]**. Altrimenti cambia in **[!UICONTROL False]**

* Quando viene creato un contatto O quando il campo dell&#39;indirizzo e-mail del contatto viene aggiornato, verificare se il contatto dispone di un indirizzo e-mail e, in caso affermativo, modificare Sync in Mkto in **[!UICONTROL True]** e cambiare Sync in Mkto in **[!UICONTROL True]** nel record Account. In caso contrario, modifica in **[!UICONTROL False]**

* Quando il campo Nome società del contatto (parentcustomerid) viene aggiornato, verifica se il campo Sync to Mkto del contatto è true. In caso affermativo, impostare Sync su Mkto sull&#39;account su **[!UICONTROL True]**
* Quando viene aggiornato il campo del potenziale cliente dell’opportunità (customerid) o del contatto (parentcontactid), verifica se il campo Sync to Mkto dell’account è true o se il campo Sync to Mkto del contatto è true. In caso affermativo, modificare Sync in Mkto sull&#39;opportunità in **[!UICONTROL True]** anche
