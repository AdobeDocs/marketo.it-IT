---
description: Scopri come configurare la sicurezza di Dynamic Chat con i domini bloccati o consentiti. Limita la visualizzazione degli agenti dei domini e-mail e i siti che possono utilizzare lo script di chat.
title: Impostazioni di sicurezza
feature: Dynamic Chat
exl-id: 68a53986-6f42-4aa2-86f6-0b2097f94963
TQID: https://experienceleague.adobe.com/7ans6J5WCXbTalK7ubMCrWBLWaJm3prPCoxsrCWEKtg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 88949407423d12a95bf39470e3c29835d934e2f6
workflow-type: tm+mt
source-wordcount: 238
ht-degree: 3%

---

# Impostazioni di sicurezza {#security-settings}

Nelle impostazioni di protezione è possibile aggiungere domini a un elenco Consentiti o a un blocco.

![](assets/security-settings-1.png)

>[!IMPORTANT]
>
>Il filtro Blocca e consenti dominio e-mail si applica solo quando un visitatore inserisce il proprio indirizzo e-mail direttamente in Dynamic Chat, nel chatbot o in un flusso di conversazione. Non si applica agli indirizzi e-mail che Dynamic Chat riceve da prodotti integrati, come Marketo Engage. Per ulteriori informazioni, consulta la tabella seguente.

| Scenario | Il filtro è applicabile? |
|---|---|
| Il visitatore digita la propria e-mail direttamente nel chatbot di Dynamic Chat | Sì |
| Il visitatore digita la propria e-mail direttamente in un flusso di conversazione Dynamic Chat | Sì |
| L’e-mail viene precompilata dall’invio di un modulo Marketo (il flusso conversazionale viene visualizzato dopo la compilazione del modulo) | No |
| L&#39;e-mail viene passata a Dynamic Chat da qualsiasi altro sistema integrato | No |

## Domini e-mail bloccati {#blocked-email-domains}

Se ci sono visitatori con domini e-mail con i quali non desideri che i tuoi agenti interagiscano (ad esempio, un concorrente), aggiungi il loro dominio e-mail al inserisco nell&#39;elenco Bloccati di.

1. Seleziona il cursore **Abilita convalida** per attivare il inserisco nell&#39;elenco Bloccati di. Immetti fino a 50 domini e fai clic su **Salva**.

   ![](assets/security-settings-2.png)

## Domini consentiti {#allowed-domains}

L’aggiunta di domini consentiti impedisce a terze parti di eliminare il JavaScript dal sito e di aggiungerlo al proprio.

1. Seleziona il cursore **Abilita convalida** per attivare il inserisco nell&#39;elenco Consentiti di. Immettere i domini consentiti e fare clic su **Salva**.

   ![](assets/security-settings-3.png)
