---
unique-page-id: 45417322
description: Eliminazione di un lead o di un contatto - Documenti Marketo - Documentazione del prodotto
title: Eliminazione di un lead o di un contatto
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# Eliminazione di un lead o di un contatto {#deleting-a-lead-or-contact}

Ci sono alcune cose da sapere quando si tratta di eliminare i lead/contatti in Microsoft Dynamics.

* Marketo non elimina automaticamente le persone solo perché i lead sono stati eliminati in Dynamics. Piuttosto, un flag &quot;Microsoft è eliminato&quot; è impostato su true. Se lo desideri, puoi attivare questo campo per eliminare il record in Marketo.

* Azione di flusso &quot;Elimina persona&quot;: Questo elimina solo una persona in Marketo (un’opzione per eliminarla anche in Dynamics non è disponibile).

* Se un lead viene eliminato in Marketo (ma non in Dynamics) e viene aggiornato in Dynamics in seguito, creerà una nuova persona in Marketo (stesso indirizzo e-mail, nuovo ID persona).

* Se un lead viene eliminato in Dynamics (ma non in Marketo) ed eseguito successivamente tramite l’azione di flusso &quot;Sincronizza persona con Microsoft&quot;, creerebbe un nuovo lead in Dynamics.
