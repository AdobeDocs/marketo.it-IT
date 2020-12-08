---
unique-page-id: 10095307
description: Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail - Documenti Marketo - Documentazione prodotto
title: Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail {#custom-sync-filter-rules-for-an-email-address}

Per evitare la sincronizzazione di record privi di indirizzo e-mail, segui queste regole.

* Quando viene creato un lead O quando il campo dell’indirizzo e-mail del lead viene aggiornato, verificate che il lead disponga di un indirizzo e-mail e, in caso contrario, modificate l’opzione Sincronizza con Mkto su **True**. In caso contrario, passa a **False**

* Quando viene creato un contatto O quando il campo dell&#39;indirizzo e-mail del contatto viene aggiornato, verificate che il contatto disponga di un indirizzo e-mail e, in caso affermativo, modificate Sincronizza con Mkto su **True** e modificate Sincronizza con Mkto su **True** nel record Account. In caso contrario, passa a **False**

* Quando il campo Nome società (parentcustomerid) del contatto viene aggiornato, verificate che il campo Sincronizzazione su Mkto del contatto sia true. Se lo è, imposta anche **True** su Mkto per l&#39;account
* Quando il campo Customer (customerid) dell’opportunità o Contact (parentcontactid) viene aggiornato, verificate che il campo Sync to Mkto dell’account sia true o che il campo Sync to Mkto del contatto sia true. Se lo è, cambia Sincronizza con Mkto sull&#39;opportunità di **True** anche

