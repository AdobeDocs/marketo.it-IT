---
unique-page-id: 11377395
description: Aggiungere un dominio di branding aggiuntivo - Documentazione di Marketo - Documentazione di prodotto
title: Aggiungi un dominio di branding aggiuntivo
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: dafac137a6c626794f3b9b2bfaa2fc2de9f2cb75
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 1%

---

# Aggiungi un dominio di branding aggiuntivo {#add-an-additional-branding-domain}

Aggiungi un dominio di branding aggiuntivo quando esegui più marchi da una singola istanza di Marketo e vuoi che ciascuno di essi abbia i propri collegamenti di tracciamento del brand.

>[!PREREQUISITES]
>
>È necessario [sostituire il collegamento di tracciamento generico](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"} con un dominio con marchio prima di aggiungere altri domini con marchio.

1. Passare all&#39;area **[!UICONTROL Admin]**.

   ![](assets/add-an-additional-branding-domain-1.png)

1. Fai clic su **[!UICONTROL Email]**.

   ![](assets/add-an-additional-branding-domain-2.png)

1. Fare clic su **[!UICONTROL Add]** per aggiungere un dominio di branding aggiuntivo.

   ![](assets/add-an-additional-branding-domain-3.png)

1. Immettere il nome del nuovo dominio di branding, selezionare _Rendi dominio primario_ e/o _Genera certificato SSL_ (entrambi facoltativi) e fare clic su **[!UICONTROL Save]**.

   ![](assets/add-an-additional-branding-domain-4.png)

>[!NOTE]
>
>* _Rendi dominio primario_: imposta questo dominio primario come dominio principale e tutti i messaggi e-mail non inviati esistenti su &quot;Predefinito&quot;; tutti i messaggi e-mail appena creati verranno impostati come dominio primario come predefinito. Puoi [sovrascriverlo per ogni e-mail](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/overwrite-primary-domain-for-emails.md){target="_blank"}.
>
>* _Genera certificato SSL_: è possibile creare un SSL (Secure Sockets Layer) con la creazione del dominio. Il primo dominio di tracciamento avvierà la configurazione una tantum dell’infrastruttura, che potrebbe richiedere alcune ore. Riceverai una notifica al termine dell’operazione e potrai quindi impostare il primo dominio. Per aggiungere SSL ai domini esistenti, contattare il [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

## Messaggi di errore {#error-messages}

<table><thead>
  <tr>
    <th>Errore</th>
    <th>Dettagli</th>
  </tr></thead>
<tbody>
  <tr>
    <td><i>Errore imprevisto durante la creazione di un dominio. Contatta il supporto per assistenza.</i></td>
    <td>Si è verificato un errore imprevisto. Raccogliere i registri e i dettagli degli errori e inoltrare il problema al <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Supporto Marketo</a>.</td>
  </tr>
  <tr>
    <td><i>Il certificato SSL è già stato rilasciato.</i></td>
    <td>Esiste già un certificato SSL per questo dominio personalizzato. Non sono necessarie ulteriori azioni a meno che il certificato non sia scaduto o debba essere nuovamente rilasciato.</td>
  </tr>
  <tr>
    <td><i>Il dominio non è mappato al dominio predefinito.</i></td>
    <td>Il dominio personalizzato non è mappato correttamente al dominio predefinito. Verificare le impostazioni di mappatura del dominio e assicurarsi che la configurazione DNS punti al dominio predefinito corretto.</td>
  </tr>
  <tr>
    <td><i>La configurazione di Cloudflare è stata avviata. Riprova più tardi.</i></td>
    <td>Quando crei il primo dominio di tracciamento per l’istanza, in Cloud viene eseguita una configurazione dell’infrastruttura una tantum. Questo messaggio indica che la configurazione è stata avviata e può richiedere fino a tre ore.</td>
  </tr>
  <tr>
    <td><i>La configurazione di Cloudflare è ancora in corso. Riprova più tardi.</i></td>
    <td>vedi sopra</td>
  </tr>
  <tr>
    <td><i>Configurazione di Cloudflare non riuscita a causa di un errore imprevisto. Contatta l’assistenza clienti.</i></td>
    <td>Configurazione iniziale dell'infrastruttura cloud non riuscita. Rivolgiti al <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Supporto Marketo</a> per assistenza.</td>
  </tr>
</tbody></table>

## Aspetti da considerare {#things-to-note}

* **Mappatura DNS per il dominio in Marketo Engage**: prima di aggiungere domini nell&#39;interfaccia utente, è necessario [mappare i CNAME in un dominio fornito da Marketo](https://experienceleague.adobe.com/it/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **SSL personalizzati**: se hai bisogno di un SSL personalizzato, invia un [ticket di supporto](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Non utilizzare la casella di controllo self-service per la creazione SSL.

* **SSL preesistenti**: durante l&#39;aggiunta di un dominio, il sistema verifica la presenza di SSL preesistenti, che potrebbero essere stati creati manualmente in precedenza. Se si verifica questa convalida, crea il dominio senza selezionare la creazione SSL, che verrà connessa automaticamente. [Contatta il supporto](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} per ulteriori dettagli/opzioni.

* **Primo dominio di tracciamento**: la prima creazione dei domini di collegamento di tracciamento e-mail richiederà l&#39;intervento manuale del [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. La successiva creazione di sottodomini nello stesso dominio è consentita nell’interfaccia utente di.

* **Aggiunta di certificati a domini esistenti**: l&#39;aggiunta di certificati a domini esistenti non è al momento supportata. Per i domini preesistenti o per i casi in cui non è stato possibile selezionare la casella del certificato SSL, è necessario contattare il [supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} per ottenere l&#39;aggiunta del certificato.

* **Modifica o rimozione di certificati nei domini esistenti**: se è necessario aggiornare o rimuovere un SSL esistente, contattare il [supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* **Eliminazione di domini**: l&#39;eliminazione di un dominio non comporta l&#39;eliminazione automatica del certificato SSL in questo momento. Questo problema sarà risolto in una versione futura.

>[!MORELIKETHIS]
>
>[Modifica il dominio di branding predefinito](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
