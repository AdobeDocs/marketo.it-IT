---
unique-page-id: 2359918
description: Modifica impostazioni pagina di destinazione - Documentazione di Marketo - Documentazione del prodotto
title: Modifica impostazioni pagina di destinazione
exl-id: 019b4651-3a66-46f9-8722-66af30194380
source-git-commit: b71729a678ff4a676bb60803d845d0a44118f7e5
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 1%

---

# Modifica impostazioni pagina di destinazione {#edit-landing-page-settings}

Puoi modificare il nome di dominio e la pagina di fallback, abilitare o disabilitare la precompilazione dei moduli, evitare l’uso improprio della pagina di destinazione e altro ancora. Ecco come.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/edit-landing-page-settings-1.png)

1. Clic **[!UICONTROL Pagine di destinazione]**.

   ![](assets/edit-landing-page-settings-2.png)

1. In **[!UICONTROL Pagine di destinazione]** , fare clic su **[!UICONTROL Modifica]**.

   ![](assets/edit-landing-page-settings-3.png)

1. Immetti il dominio e le informazioni sulla pagina.

   ![](assets/edit-landing-page-settings-4.png)

   | Termine | Definizione |
   |---|---|
   | [!UICONTROL Nome di dominio per le pagine di destinazione] | Questo è il tuo CNAME. Un CNAME è la prima parte dell’URL che viene assegnato alle persone per le pagine di destinazione. Ad esempio, in `https://go.yourCompany.com`, la parola &quot;go&quot; è il CNAME. Si possono avere più, ma la maggior parte delle persone usa solo quello. |
   | [!UICONTROL Pagina di fallback] | Questo è il percorso da seguire se la pagina di destinazione non esiste o è inattiva. Ulteriori informazioni su [pagine di fallback](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | [!UICONTROL Home page] | Immetti l’URL del sito aziendale. |

1. Controlla la **[!UICONTROL Precompilazione modulo]** casella di controllo per consentire ai moduli di precompilare le informazioni per le persone note (ricette). Deseleziona per bloccare.

   ![](assets/edit-landing-page-settings-5.png)

1. Se vuoi evitare che un sito dannoso ospiti apparentemente il tuo contenuto, controlla **[!UICONTROL Non consentire l’incorporamento di pagine Marketo in pagine web esterne]** casella di controllo.

   ![](assets/edit-landing-page-settings-6.png)

   >[!NOTE]
   >
   >Se si desidera la precompilazione `<script>` da visualizzare alla fine del `<head>` nel codice, controlla **[!UICONTROL Inserisci script di preriempimento alla fine dell’intestazione]** casella. Lascia deselezionata questa opzione per visualizzarla all’inizio.
   >
   >Verifica **[!UICONTROL Rimuovi collegamenti favicon predefiniti]** per impedire a Marketo di inserire collegamenti favicon nel codice.

1. Dopo aver effettuato le selezioni, fai clic su **[!UICONTROL Salva]**.

   ![](assets/edit-landing-page-settings-7.png)

   Ottimo lavoro! Le pagine di destinazione ora dispongono delle informazioni corrette e dovrebbero iniziare a funzionare immediatamente.
