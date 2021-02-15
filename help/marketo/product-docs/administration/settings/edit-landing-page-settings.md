---
unique-page-id: 2359918
description: Modifica impostazioni pagina di destinazione - Documenti Marketo - Documentazione prodotto
title: Modifica impostazioni pagina di destinazione
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Modifica impostazioni pagina di destinazione {#edit-landing-page-settings}

È possibile modificare il nome di dominio e la pagina di fallback, abilitare o disabilitare la precompilazione del modulo, impedire l&#39;uso improprio della pagina di destinazione e altro ancora. Ecco come.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. In **Admin**, fare clic su **Pagine di destinazione**.

   ![](assets/image2014-9-10-9-3a47-3a40.png)

1. Nella sezione **Pagine di destinazione**, fare clic su **Modifica**.

   ![](assets/image2014-9-10-9-3a47-3a12.png)

1. Immettete il dominio e le informazioni sulla pagina.

   | Termine | Definizione |
   |---|---|
   | Nome di dominio per le pagine di destinazione | Questo è il tuo CNAME. Un CNAME è la prima parte dell’URL che date alle persone per le pagine di destinazione. Ad esempio, in `https://go.yourCompany.com`, la parola &quot;go&quot; è il CNAME. Puoi avere più persone, ma la maggior parte usa solo quella. |
   | Pagina di fallback | Indica dove andare se la pagina di destinazione non esiste o è inattiva. Ulteriori informazioni su [pagine di fallback](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | Homepage | Immettete l’URL del sito aziendale. |

   ![](assets/three.png)

1. Selezionare la casella di controllo **Precompila modulo** per consentire ai moduli di precompilare le informazioni per le persone conosciute (sottoposte a cookie). Deselezionare per bloccare.

   ![](assets/four.png)

1. Per evitare che un sito dannoso possa ospitare contenuti, selezionare la casella di controllo **Non consentire l&#39;incorporazione di pagine Web esterne**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Se desiderate che il tag precompila `<script>` venga visualizzato alla fine del tag `<head>` nel codice, selezionate la casella **Inserisci script di precompilazione alla fine della testina**. Lasciate deselezionata se desiderate che appaia all&#39;inizio.
   >
   >Selezionare **Rimuovi i collegamenti preferiti predefiniti** per evitare che Marketo inserisca eventuali collegamenti preferiti nel codice.

1. Dopo aver effettuato le selezioni, fare clic su **Salva.**

   ![](assets/six.png)

   Ottimo lavoro! Le pagine di destinazione ora dispongono delle informazioni giuste e dovrebbero iniziare a funzionare immediatamente.
