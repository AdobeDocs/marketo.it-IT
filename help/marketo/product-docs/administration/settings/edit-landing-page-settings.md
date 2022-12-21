---
unique-page-id: 2359918
description: Modifica impostazioni pagina di destinazione - Documentazione Marketo - Documentazione del prodotto
title: Modifica impostazioni pagina di destinazione
exl-id: 019b4651-3a66-46f9-8722-66af30194380
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Modifica impostazioni pagina di destinazione {#edit-landing-page-settings}

Puoi modificare il nome di dominio e la pagina di fallback, abilitare o disabilitare la precompilazione del modulo, evitare l’uso improprio della pagina di destinazione e altro ancora. Ecco come.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Sotto **Amministratore**, fai clic su **Pagine di destinazione**.

   ![](assets/image2014-9-10-9-3a47-3a40.png)

1. In **Pagine di destinazione** sezione, fai clic su **Modifica**.

   ![](assets/image2014-9-10-9-3a47-3a12.png)

1. Immetti il dominio e le informazioni sulla pagina.

   | Termine | Definizione |
   |---|---|
   | Nome di dominio per le pagine di destinazione | Questo è il tuo CNAME. Un CNAME è la prima parte dell’URL che date alle persone per le pagine di destinazione. Ad esempio, in `https://go.yourCompany.com`, la parola &quot;go&quot; è il CNAME. Puoi averne diversi, ma la maggior parte delle persone usa solo quello. |
   | Pagina di fallback | Se la pagina di destinazione non esiste o è inattiva, verrà visualizzata la seguente pagina. Ulteriori informazioni [pagine di fallback](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | Home page | Inserisci l&#39;URL del sito aziendale. |

   ![](assets/three.png)

1. Controlla la **Precompilazione modulo** per consentire ai moduli di precompilare le informazioni per le persone note (cookie). Deseleziona per bloccare.

   ![](assets/four.png)

1. Per evitare che un sito dannoso possa apparentemente ospitare i contenuti, controlla la **Non consentire l’incorporazione di pagine Marketo in pagine web esterne** casella di controllo.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Se vuoi la precompilazione `<script>` da visualizzare alla fine del `<head>` nel codice, controlla il **Inserisci script di precompilazione alla fine dell&#39;intestazione** scatola. Lascia deselezionata questa opzione se desideri che venga visualizzata all’inizio.
   >
   >Controlla **Rimuovi i collegamenti preferiti predefiniti** per impedire a Marketo di inserire nel codice eventuali collegamenti preferiti.

1. Dopo aver effettuato le selezioni, fai clic su **Salva.**

   ![](assets/six.png)

   Ottimo lavoro! Le pagine di destinazione ora dispongono delle informazioni giuste e devono iniziare a funzionare immediatamente.
