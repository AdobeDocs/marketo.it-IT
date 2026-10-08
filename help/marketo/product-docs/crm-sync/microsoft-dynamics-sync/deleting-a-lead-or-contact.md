---
unique-page-id: 45417322
description: Comprendere come funziona l’eliminazione di lead e contatti tra Microsoft Dynamics e Marketo. Utilizza il flag Microsoft is Deleted e l’azione di flusso Delete Person (Elimina persona) secondo necessità.
title: Eliminazione di un lead o di un contatto
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/4BwBuLQFJ2pRehuS8EqW-UrEcg5sVeqcstu3azh0NvQ'
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
source-wordcount: '167'
ht-degree: 5%
---
# Eliminazione di un lead o di un contatto {#deleting-a-lead-or-contact}

Ci sono alcune informazioni da sapere quando si tratta di eliminare lead/contatti in [!DNL Microsoft Dynamics].

* Marketo non elimina automaticamente le persone solo perché i lead sono stati eliminati in [!DNL Dynamics]. Piuttosto, il flag &quot;Microsoft is Deleted&quot; del campo è impostato su true. Se necessario, puoi disattivare questo campo per eliminare il record in Marketo.

* Azione di flusso &quot;Elimina persona&quot;: questa azione elimina solo una persona in Marketo (non è disponibile un’opzione per eliminarla anche in Dynamics).

* Se un lead viene eliminato in Marketo (ma non in [!DNL Dynamics]) e aggiornato successivamente in [!DNL Dynamics], verrà creata una nuova persona in Marketo (stesso indirizzo e-mail, nuovo ID persona).

* Se un lead viene eliminato in [!DNL Dynamics] (ma non in Marketo) e successivamente viene eseguito tramite l&#39;azione di flusso &quot;Sincronizza persona in Microsoft&quot;, verrà creato un nuovo lead in [!DNL Dynamics].
