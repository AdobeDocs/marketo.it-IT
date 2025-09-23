---
description: Regole di convalida modulo globale - Documentazione di Marketo - Documentazione del prodotto
title: Regole di convalida del modulo globale
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 4%

---

# Regole di convalida del modulo globale {#global-form-validation-rules}

Questa funzione consente di bloccare l&#39;invio a Marketo Engage Form di domini specifici.

## Come abilitare l’accesso {#how-to-enable-access}

Prima di poter utilizzare questa funzione, devi abilitarne l’autorizzazione per il ruolo desiderato.

1. In Marketo, fare clic su **[!UICONTROL Admin]**.

   ![](assets/global-form-validation-rules-1.png)

1. Fai clic su **[!UICONTROL Users & Roles]**.

   ![](assets/global-form-validation-rules-2.png)

1. Fare clic sulla scheda **[!UICONTROL Roles]**.

   ![](assets/global-form-validation-rules-3.png)

1. Fare doppio clic sul ruolo a cui si desidera concedere le autorizzazioni.

   ![](assets/global-form-validation-rules-4.png)

1. Fai clic sul segno **+** accanto a **Access Admin**.

   ![](assets/global-form-validation-rules-5.png)

1. Scorri verso il basso e seleziona **[!UICONTROL Access Form Validation Rules]**, quindi fai clic su **[!UICONTROL Save]**.

   ![](assets/global-form-validation-rules-6.png)

## Crea nuova regola di convalida modulo {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Queste regole verranno applicate a tutti i moduli delle sottoscrizioni Marketo Engage.

1. In Marketo, fare clic su **[!UICONTROL Admin]**.

   ![](assets/global-form-validation-rules-7.png)

1. Fai clic su **[!UICONTROL Global Form Validation Rule]**.

   ![](assets/global-form-validation-rules-8.png)

1. Fai clic su **[!UICONTROL New Form Validation Rule]**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >L&#39;elenco a discesa [!UICONTROL Form Validation Rule Actions] consente di eliminare o modificare le regole esistenti.

1. Assegna un nome alla regola, fornisci una descrizione facoltativa e inserisci il messaggio di errore che desideri venga visualizzato dai visitatori del modulo. Immettere i domini da bloccare nella casella delle regole, selezionare **[!UICONTROL Activate Rule]** e fare clic su **[!UICONTROL Create]**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage dispone di un elenco Bloccati definito di domini e-mail consumer gratuiti che vengono bloccati quando si utilizza la regola precaricata &quot;Dominio e-mail consumer: Inserire nell&#39;elenco Bloccati&quot;. [Visualizza l&#39;elenco](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv) (per scaricare, assicurati che il browser sia aggiornato e in grado di accettare i download).

## Disattivazione dell&#39;accesso per modulo{#how-to-disable-access-per-form}

Una volta abilitate, le regole vengono applicate a tutti i moduli. Se tuttavia si dispone di un modulo con requisiti specifici e non si desidera rifiutare nulla, è possibile disabilitare [!UICONTROL Global Form Validation Rules] nelle impostazioni del modulo.

1. Nella forma desiderata, fai clic su **[!UICONTROL Form Settings]**, quindi su **[!UICONTROL Settings]**.

   ![](assets/global-form-validation-rules-11.png)

1. Fare clic sull&#39;elenco a discesa **[!UICONTROL Global Form Validation Rules]** e scegliere **[!UICONTROL Disabled]**.

   ![](assets/global-form-validation-rules-12.png)

Quando approvi e pubblichi il modulo, questo ignorerà [!UICONTROL Global Form Validation Rules].
