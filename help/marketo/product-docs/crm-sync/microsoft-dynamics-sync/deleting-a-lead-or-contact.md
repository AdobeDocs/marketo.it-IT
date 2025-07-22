---
unique-page-id: 45417322
description: Eliminazione di un lead o di un contatto - Documenti Marketo - Documentazione del prodotto
title: Eliminazione di un lead o di un contatto
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Eliminazione di un lead o di un contatto {#deleting-a-lead-or-contact}

Ci sono alcune informazioni da sapere quando si tratta di eliminare lead/contatti in [!DNL Microsoft Dynamics].

* Marketo non elimina automaticamente le persone solo perché i lead sono stati eliminati in [!DNL Dynamics]. Piuttosto, il flag &quot;Microsoft is Deleted&quot; del campo è impostato su true. Se necessario, puoi disattivare questo campo per eliminare il record in Marketo.

* Azione di flusso &quot;Elimina persona&quot;: questa azione elimina solo una persona in Marketo (non è disponibile un’opzione per eliminarla anche in Dynamics).

* Se un lead viene eliminato in Marketo (ma non in [!DNL Dynamics]) e aggiornato successivamente in [!DNL Dynamics], verrà creata una nuova persona in Marketo (stesso indirizzo e-mail, nuovo ID persona).

* Se un lead viene eliminato in [!DNL Dynamics] (ma non in Marketo) e successivamente viene eseguito tramite l&#39;azione di flusso &quot;Sincronizza persona in Microsoft&quot;, verrà creato un nuovo lead in [!DNL Dynamics].
