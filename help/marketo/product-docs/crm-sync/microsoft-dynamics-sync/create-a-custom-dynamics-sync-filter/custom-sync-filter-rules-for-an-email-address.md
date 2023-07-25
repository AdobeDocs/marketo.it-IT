---
unique-page-id: 10095307
description: Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail {#custom-sync-filter-rules-for-an-email-address}

Per evitare la sincronizzazione di record privi di indirizzo e-mail, attieniti a queste regole.

* Quando viene creato un lead OPPURE quando il campo dell’indirizzo e-mail del lead viene aggiornato, verifica se il lead ha un indirizzo e-mail e, in caso affermativo, modifica Sincronizza con Mkto in **Vero**. Altrimenti modifica in **Falso**

* Quando viene creato un contatto O quando il campo dell’indirizzo e-mail del contatto viene aggiornato, verifica se il contatto dispone di un indirizzo e-mail e, in caso affermativo, modifica Sincronizza con Mkto in **Vero** e cambia da Sincronizza a Mkto a **Vero** nel record Account. In caso contrario, modifica in **Falso**

* Quando il campo Nome società del contatto (parentcustomerid) viene aggiornato, verifica se il campo Sync to Mkto del contatto è true. In caso affermativo, impostare Sincronizza su Mkto sull&#39;account in **Vero** anche
* Quando viene aggiornato il campo del potenziale cliente dell’opportunità (customerid) o del contatto (parentcontactid), verifica se il campo Sync to Mkto dell’account è true o se il campo Sync to Mkto del contatto è true. In caso affermativo, modifica Sync in Mkto sull’opportunità in **Vero** anche
