---
unique-page-id: 10095307
description: Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail - Documenti Marketo - Documentazione prodotto
title: Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail {#custom-sync-filter-rules-for-an-email-address}

Per evitare la sincronizzazione di record privi di indirizzo e-mail, segui queste regole.

* Quando viene creato un lead O quando il campo dell’indirizzo e-mail del lead viene aggiornato, verificate che il lead disponga di un indirizzo e-mail e, in caso affermativo, modificate Sincronizza con Mkto in **True**. In caso contrario, passare a **False**

* Quando viene creato un contatto O quando il campo dell&#39;indirizzo e-mail del contatto viene aggiornato, verificare che il contatto disponga di un indirizzo e-mail e, in caso affermativo, modificare l&#39;opzione Sincronizza con Mkto in **True** e impostare l&#39;opzione Sincronizza con Mkto su **True** nel record Account. In caso contrario, passare a **False**

* Quando il campo Nome società (parentcustomerid) del contatto viene aggiornato, verificate che il campo Sincronizzazione su Mkto del contatto sia true. Se lo è, cambiare Sincronizzazione su Mkto sull&#39;account su **True** anche
* Quando il campo Customer (customerid) dell’opportunità o Contact (parentcontactid) viene aggiornato, verificate che il campo Sync to Mkto dell’account sia true o che il campo Sync to Mkto del contatto sia true. Se lo è, cambiare Sincronizzazione su Mkto sull&#39;opportunità di **True** anche
