---
unique-page-id: 45417322
description: Eliminazione di un lead o di un contatto - Documenti Marketo - Documentazione del prodotto
title: Eliminazione di un lead o di un contatto
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# Eliminazione di un lead o di un contatto {#deleting-a-lead-or-contact}

Quando si tratta di eliminare lead/contatti in Microsoft Dynamics, è necessario conoscere alcuni aspetti.

* Marketo non elimina automaticamente le persone solo perché i lead sono stati eliminati in Dynamics. Piuttosto, il flag &quot;Microsoft is Deleted&quot; del campo è impostato su true. Se necessario, puoi disattivare questo campo per eliminare il record in Marketo.

* Azione di flusso &quot;Elimina persona&quot;: questa azione elimina solo una persona in Marketo (non è disponibile un’opzione per eliminarla anche in Dynamics).

* Se un lead viene eliminato in Marketo (ma non in Dynamics) e successivamente viene aggiornato in Dynamics, verrà creata una nuova persona in Marketo (stesso indirizzo e-mail, nuovo ID persona).

* Se un lead viene eliminato in Dynamics (ma non in Marketo) e successivamente viene eseguito tramite l’azione di flusso &quot;Sincronizza persona in Microsoft&quot;, verrà creato un nuovo lead in Dynamics.
