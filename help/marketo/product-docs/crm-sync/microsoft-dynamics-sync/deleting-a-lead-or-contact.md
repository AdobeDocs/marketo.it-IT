---
unique-page-id: 45417322
description: Eliminazione di un lead o di un contatto - Documenti Marketo - Documentazione prodotto
title: Eliminazione di un lead o di un contatto
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Eliminazione di un lead o di un contatto {#deleting-a-lead-or-contact}

Ci sono alcune cose da sapere quando si tratta di eliminare i lead/contatti in Microsoft Dynamics.

* Marketo non elimina automaticamente le persone solo perché i lead sono stati eliminati in Dynamics. Piuttosto, il flag &quot;Microsoft is Deleted&quot; del campo è impostato su true. Se necessario, è possibile attivare il campo per eliminare il record in Marketo.

* Azione flusso &quot;Elimina persona&quot;: Questo elimina solo una persona in Marketo (un&#39;opzione per eliminarla anche in Dynamics non è disponibile).

* Se un lead viene eliminato in Marketo (ma non in Dynamics) e aggiornato in Dynamics dopo tale data, creerà una nuova persona in Marketo (stesso indirizzo e-mail, nuovo ID persona).

* Se un lead viene eliminato in Dynamics (ma non in Marketo) ed eseguito successivamente tramite l’azione di flusso &quot;Sincronizza persona con Microsoft&quot;, creerebbe un nuovo lead in Dynamics.
