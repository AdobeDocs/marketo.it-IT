---
description: Regole di convalida modulo globale - Documentazione di Marketo - Documentazione del prodotto
title: Regole di convalida modulo globale
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Regole di convalida modulo globale {#global-form-validation-rules}

Questa funzione consente di bloccare l’invio di domini specifici ai moduli del Marketo Engage.

## Come abilitare l’accesso {#how-to-enable-access}

Prima di poter utilizzare questa funzione, devi abilitarne l’autorizzazione per il ruolo desiderato.

1. In Marketo, fai clic su **[!UICONTROL Amministratore]**.

   ![](assets/global-form-validation-rules-1.png)

1. Clic **[!UICONTROL Utenti e ruoli]**.

   ![](assets/global-form-validation-rules-2.png)

1. Fai clic su **[!UICONTROL Ruoli]** scheda.

   ![](assets/global-form-validation-rules-3.png)

1. Fare doppio clic sul ruolo a cui si desidera concedere le autorizzazioni.

   ![](assets/global-form-validation-rules-4.png)

1. Fai clic su **+** Accedi ad Access Admin.

   ![](assets/global-form-validation-rules-5.png)

1. Scorri verso il basso e seleziona **[!UICONTROL Regole di convalida modulo di accesso]** e fai clic su **[!UICONTROL Salva]**.

   ![](assets/global-form-validation-rules-6.png)

## Crea nuova regola di convalida modulo {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Queste regole verranno applicate a tutti i moduli delle sottoscrizioni di Marketo Engage.

1. In Marketo, fai clic su **[!UICONTROL Amministratore]**.

   ![](assets/global-form-validation-rules-7.png)

1. Clic **[!UICONTROL Regola di convalida modulo globale]**.

   ![](assets/global-form-validation-rules-8.png)

1. Clic **[!UICONTROL Nuova regola di convalida modulo]**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >Il menu a discesa Azioni regola di convalida modulo consente di eliminare o modificare le regole esistenti.

1. Assegna un nome alla regola, fornisci una descrizione facoltativa e inserisci il messaggio di errore che desideri venga visualizzato dai visitatori del modulo. Immetti i domini da bloccare nella casella delle regole, seleziona **[!UICONTROL Attiva regola]** e fai clic su **[!UICONTROL Crea]**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Il Marketo Engage dispone di un elenco Bloccati definito di domini e-mail consumer gratuiti che vengono bloccati quando si utilizza la regola di Elenco Bloccati del dominio e-mail consumer pre-caricata &quot;Dominio e-mail consumer:&quot;. [Visualizza l&#39;elenco](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv).

## Disattivazione dell&#39;accesso per modulo{#how-to-disable-access-per-form}

Una volta abilitate, le regole vengono applicate a tutti i moduli. Se tuttavia si dispone di un modulo con requisiti specifici e non si desidera che venga rifiutato alcun elemento, è possibile disattivare [!UICONTROL Regole di convalida modulo globale] nelle impostazioni del modulo.

1. Nel modulo desiderato, fai clic su **[!UICONTROL Impostazioni modulo]**, quindi **[!UICONTROL Impostazioni]**.

   ![](assets/global-form-validation-rules-11.png)

1. Fai clic su **[!UICONTROL Regole di convalida modulo globale]** e scegliere **[!UICONTROL Disabilitato]**.

   ![](assets/global-form-validation-rules-12.png)

Quando approvi e pubblichi il modulo, questo ignorerà il tuo [!UICONTROL Regole di convalida modulo globale].
