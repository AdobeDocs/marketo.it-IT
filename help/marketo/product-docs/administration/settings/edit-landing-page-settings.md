---
unique-page-id: 2359918
description: Modifica impostazioni pagina di destinazione - Documentazione di Marketo - Documentazione del prodotto
title: Modificare le impostazioni della pagina di destinazione
exl-id: 019b4651-3a66-46f9-8722-66af30194380
feature: Administration, Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 9%

---

# Modificare le impostazioni della pagina di destinazione {#edit-landing-page-settings}

Puoi modificare il nome di dominio e la pagina di fallback, abilitare o disabilitare la precompilazione dei moduli, evitare l’uso improprio della pagina di destinazione e altro ancora. Ecco come.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/edit-landing-page-settings-1.png)

1. Fai clic su **[!UICONTROL Landing Pages]**.

   ![](assets/edit-landing-page-settings-2.png)

1. Nella sezione **[!UICONTROL Landing Pages]**, fare clic su **[!UICONTROL Edit]**.

   ![](assets/edit-landing-page-settings-3.png)

1. Immetti il dominio e le informazioni sulla pagina.

   ![](assets/edit-landing-page-settings-4.png)

   | Termine | Definizione |
   |---|---|
   | [!UICONTROL Domain name for landing pages] | Questo è il tuo CNAME. Un CNAME è la prima parte dell’URL che viene assegnato alle persone per le pagine di destinazione. In `https://go.yourCompany.com`, ad esempio, la parola &quot;go&quot; è il CNAME. Si possono avere più, ma la maggior parte delle persone usa solo quello. |
   | [!UICONTROL Fallback page] | Questo è il percorso da seguire se la pagina di destinazione non esiste o è inattiva. Ulteriori informazioni su [pagine di fallback](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | [!UICONTROL Homepage] | Immetti l’URL del sito aziendale. |

1. Selezionare la casella di controllo **[!UICONTROL Form Prefill]** per consentire ai moduli di precompilare le informazioni per le persone note (con cookie). Deseleziona per bloccare.

   ![](assets/edit-landing-page-settings-5.png)

   >[!NOTE]
   >
   >Se si desidera che il tag di precompilazione `<script>` venga visualizzato alla fine del tag `<head>` nel codice, selezionare la casella **[!UICONTROL Inject Prefill Script at End of Head]**. Lascia deselezionata questa opzione per visualizzarla all’inizio.
   >
   >Selezionare **[!UICONTROL Remove default favicon links]** per impedire a Marketo di inserire collegamenti favicon nel codice.

1. Dopo aver effettuato le selezioni, fare clic su **[!UICONTROL Save]**.

   ![](assets/edit-landing-page-settings-6.png)

   Ottimo lavoro! Le pagine di destinazione ora dispongono delle informazioni corrette e dovrebbero iniziare a funzionare immediatamente.
