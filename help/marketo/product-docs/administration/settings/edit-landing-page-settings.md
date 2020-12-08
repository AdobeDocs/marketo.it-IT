---
unique-page-id: 2359918
description: Modifica impostazioni pagina di destinazione - Documenti Marketo - Documentazione prodotto
title: Modifica impostazioni pagina di destinazione
translation-type: tm+mt
source-git-commit: 95ca406109e04f56c9846f83cb2c4202bf606518
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Modifica impostazioni pagina di destinazione {#edit-landing-page-settings}

È possibile modificare il nome di dominio e la pagina di fallback, abilitare o disabilitare la precompilazione del modulo, impedire l&#39;uso improprio della pagina di destinazione e altro ancora. Ecco come.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. In **Admin**, fai clic su **Pagine** di destinazione.

   ![](assets/image2014-9-10-9-3a47-3a40.png)

1. Nella sezione Pagine **di** destinazione, fate clic su **Modifica**.

   ![](assets/image2014-9-10-9-3a47-3a12.png)

1. Immettete il dominio e le informazioni sulla pagina.

   | Termine | Definizione |
   |---|---|
   | Nome di dominio per le pagine di destinazione | Questo è il tuo CNAME. Un CNAME è la prima parte dell’URL che date alle persone per le pagine di destinazione. Ad esempio, in `http://go.yourCompany.com`, la parola &quot;go&quot; è il CNAME. Puoi avere più persone, ma la maggior parte usa solo quella. |
   | Pagina di fallback | Indica dove andare se la pagina di destinazione non esiste o è inattiva. Ulteriori informazioni sulle pagine di [fallback](set-a-fallback-page.md). |
   | Homepage | Immettete l’URL del sito aziendale. |

   ![](assets/three.png)

1. Selezionare la casella di controllo Precompilazione **** modulo per consentire ai moduli di precompilare le informazioni per gli utenti noti (con cookie). Deselezionare per bloccare.

   ![](assets/four.png)

1. Se desiderate impedire a un sito dannoso di ospitare i contenuti, selezionate la casella di controllo **Non consentire l’incorporamento di pagine Marketo in pagine** Web esterne.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Se desiderate che il `<script>` tag di precompilazione venga visualizzato alla fine del `<head>` tag nel codice, selezionate la casella **Inserisci script di precompilazione alla fine della testina** . Lasciate deselezionata se desiderate che appaia all&#39;inizio.
   >
   >Selezionate **Rimuovi i collegamenti** preferiti predefiniti per evitare che Marketo inserisca eventuali collegamenti preferiti nel codice.

1. Dopo aver effettuato le selezioni, fate clic su **Salva.**

   ![](assets/six.png)

   Ottimo lavoro! Le pagine di destinazione ora dispongono delle informazioni giuste e dovrebbero iniziare a funzionare immediatamente.

