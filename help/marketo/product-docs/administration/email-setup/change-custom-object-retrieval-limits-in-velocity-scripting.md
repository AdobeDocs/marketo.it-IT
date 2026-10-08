---
description: Aumentare o diminuire il limite di recupero degli oggetti personalizzati padre per lo script [!DNL Velocity] nelle e-mail (da 10 a 100).
title: Modifica dei limiti di recupero degli oggetti personalizzati in [!DNL Velocity Scripting]
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
TQID: 'https://experienceleague.adobe.com/8zdwliEWuUxePbN3RyElJZydMfPHO8sQbgZbaTda6iY'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a03c57fb-0705-4a0d-b463-bbc931d4cefa
    internal-label: Email setup
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 1%
---
# Modifica dei limiti di recupero degli oggetti personalizzati in [!DNL Velocity Scripting] {#change-custom-object-retrieval-limits-in-velocity-scripting}

Se utilizzi [!DNL Velocity Script] per visualizzare i dati degli oggetti personalizzati nelle e-mail, questa funzione potrebbe essere applicabile al tuo caso d&#39;uso. Per impostazione predefinita, è consentito l’accesso a 10 oggetti personalizzati principali dallo script Velocity. Per ulteriori informazioni, consulta la procedura riportata di seguito.

## Cos&#39;è [!DNL Velocity] {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) è un linguaggio basato su [!DNL Java] progettato per la creazione di modelli e lo scripting del contenuto di HTML. Marketo consente di utilizzarlo nel contesto delle e-mail tramite [token di script](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Questo consente, tra l’altro, di accedere ai dati memorizzati negli oggetti personalizzati.

È possibile fare riferimento a oggetti personalizzati padre e figlio che sono direttamente connessi al lead o al contatto, ma non a oggetti personalizzati di terzo livello. Per ogni oggetto personalizzato, i 10 record aggiornati più di recente per persona/contatto sono disponibili in fase di esecuzione e vengono ordinati dall’ultimo aggiornamento (in corrispondenza di 0) a quello più recente (in corrispondenza di 9).

## Come modificare il limite {#how-to-change-the-limit}

1. Passare alla sezione **[!UICONTROL Admin]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Fai clic su **[!UICONTROL Email]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. Nella tabella [!UICONTROL Custom Object Retrieval Limits], immettere un nuovo [!UICONTROL Parent Retrieval Limit] e fare clic su **[!UICONTROL Save Changes]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>Il valore [!UICONTROL Parent Retrieval Limit] deve essere compreso tra 10 e 100. [!UICONTROL Child Retrieval Limit] viene impostato automaticamente. A tale scopo, dividere 1000 per [!UICONTROL Parent Retrieval Limit]. Ad esempio, se si imposta il limite Padre su 50, il limite Figlio diventa 20 (1000 ÷ 50 = 20).

È ora possibile accedere a più oggetti personalizzati da [!DNL Velocity script].
