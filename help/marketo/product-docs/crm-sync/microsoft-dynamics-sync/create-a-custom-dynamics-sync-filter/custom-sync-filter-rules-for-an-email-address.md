---
unique-page-id: 10095307
description: Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail - Documenti Marketo - Documentazione del prodotto
title: Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail {#custom-sync-filter-rules-for-an-email-address}

Per evitare la sincronizzazione di record privi di indirizzo e-mail, segui queste regole.

* Quando viene creato un lead O quando il campo dell’indirizzo e-mail del lead viene aggiornato, verifica se il lead dispone di un indirizzo e-mail e, in caso affermativo, modifica Sincronizza con Mkto in **True**. Altrimenti cambia in **False**

* Quando un contatto viene creato OPPURE quando il campo dell&#39;indirizzo e-mail del contatto viene aggiornato, controlla se il contatto dispone di un indirizzo e-mail e, in caso affermativo, cambia Sincronizza con Mkto in **True** e cambia Sincronizza con Mkto in **True** nel record Account. In caso contrario, passa a **False**

* Quando il campo Nome società (parentcustomerid) del contatto viene aggiornato, controlla se il campo Sincronizzazione su mkto del contatto è true. Se lo è, cambia Sincronizza con Mkto sull&#39;account in **True** anche
* Quando il campo Customer (customerid) dell’opportunità o Contact (parentcontactid) viene aggiornato, controlla se il campo Sync to Mkto dell’account è true o se il campo Sync to Mkto del contatto è true. Se lo è, cambia Sincronizza con Mkto sull&#39;opportunità di **True** anche
