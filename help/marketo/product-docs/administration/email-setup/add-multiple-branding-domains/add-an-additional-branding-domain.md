---
unique-page-id: 11377395
description: Add extra branding domains for multiple brands in one instance so each has its own branded tracking links.
title: Aggiungere un ulteriore dominio di branding
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: 6638f4a24aac6cf828f443d17b896a9dec9bca16
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 19%

---

# Aggiungere un ulteriore dominio di branding {#add-an-additional-branding-domain}

Add an additional branding domain when you&#39;re running multiple brands out of a single Marketo instance and want them each to have their own branded tracking links.

>[!PREREQUISITES]
>
>You must [replace the generic tracking link](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"} with a branded domain before adding additional branded domains.

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/add-an-additional-branding-domain-1.png)

1. Fai clic su **[!UICONTROL Email]**.

   ![](assets/add-an-additional-branding-domain-2.png)

1. Click **[!UICONTROL Add]** to add an additional branding domain.

   ![](assets/add-an-additional-branding-domain-3.png){width="600"}

1. Enter the name of your new branding domain, select _Make Primary Domain_ and/or _Generate SSL Certificate_ (both optional), and click **[!UICONTROL Save]**.

   ![](assets/add-an-additional-branding-domain-4.png)

>[!NOTE]
>
>* _Make Primary Domain_: Make this your primary domain, and all existing unsent emails set to &quot;Default&quot; and all newly created emails will default to the primary domain. You can [overwrite this on a per-email basis](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/overwrite-primary-domain-for-emails.md){target="_blank"}.
>
>* _Generate SSL Certificate_: You can create a Secure Sockets Layer (SSL) with the creation of the domain. The first tracking domain will initiate a one-time set up of infrastructure that may take a few hours. You will be notified upon completion, and you can then set up the first domain. To add SSL to your existing domains, please reach out to [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

## Edit SSLs for existing domains

Per abilitare SSL per i domini esistenti, segui la procedura riportata di seguito.

1. From the _[!UICONTROL Admin]_area, select **[!UICONTROL Email]**.

1. On the _[!UICONTROL Domain]_tab, select the domain row and click **[!UICONTROL Add SSL]**.

   ![Admin - Email - Domain - Add SSL](./assets/admin-email-branding-domain-add-ssl.png){width="600"}

1. In the dialog, click **[!UICONTROL Confirm]**.

   ![Add SSL - Confirm](./assets/generate-ssl-cert-confirm.png){width="400"}

## Error Messages {#error-messages}

<table><thead>
  <tr>
    <th>Errore</th>
    <th>Dettagli</th>
  </tr></thead>
<tbody>
<tr>
    <td><i>Domain already exists.</i></td>
    <td>Esiste già un dominio con lo stesso nome.</td>
  </tr>
  <tr>
    <td><i>Domain is not mapped to the default domain.</i></td>
    <td>Il dominio personalizzato non è mappato correttamente al dominio predefinito. Please verify the domain mapping settings and ensure the DNS configuration points to the correct default domain.</td>
  </tr>
  <tr>
    <td><i>SSL certificates could not be issued due to unsupported CAA records. Request your IT to update your CAA records.</i></td>
    <td>Record CAA non aggiornati. For those using Marketo Engage managed SSL certificates, CAA records need to be updated to certificates recommended by our vendor. Contatta il reparto IT per aggiornare i record CAA. Vedi <a href="https://nation.marketo.com/t5/product-blogs/changes-to-marketo-engage-secured-domains-platform/ba-p/329305#M2246">questa pagina</a> per ulteriori dettagli.</td>
  </tr>
  <tr>
    <td><i>Il certificato SSL è già stato rilasciato.</i></td>
    <td>Esiste già un certificato SSL per questo dominio personalizzato. Non sono necessarie ulteriori azioni a meno che il certificato non sia scaduto o debba essere nuovamente rilasciato.</td>
  </tr>
  <tr>
    <td><i>Dominio predefinito non trovato. Contatta il supporto per assistenza.</i></td>
    <td>Si è verificato un problema durante il tentativo di individuare il dominio predefinito. Rivolgiti al Supporto tecnico per consentire loro di svolgere indagini approfondite.</td>
  </tr>
  <tr>
    <td><i>Errore imprevisto durante la creazione di un dominio. Contatta il supporto per assistenza.</i></td>
    <td>Si è verificato un errore imprevisto. Raccogliere i registri e i dettagli degli errori e inoltrare il problema al <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Supporto Marketo</a>.</td>
  </tr>
</tbody></table>

## Aspetti da considerare {#things-to-note}

* **Mappatura DNS per il dominio in Marketo Engage**: prima di aggiungere domini nell&#39;interfaccia utente, è necessario [mappare i CNAME in un dominio fornito da Marketo](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **SSL personalizzati**: se hai bisogno di un SSL personalizzato, invia un [ticket di supporto](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Non utilizzare la casella di controllo self-service per la creazione SSL.

* **SSL preesistenti**: durante l&#39;aggiunta di un dominio, il sistema verifica la presenza di SSL preesistenti, che potrebbero essere stati creati manualmente in precedenza. Se si verifica questa convalida, crea il dominio senza selezionare la creazione SSL, che verrà connessa automaticamente. [Contatta il supporto](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} per ulteriori dettagli/opzioni.

* **Eliminazione di domini**: l&#39;eliminazione automatica di un dominio **non** comporta l&#39;eliminazione del certificato SSL. Questo guardrail evita errori degli utenti che determinano la mancanza di certificati SSL in un sito Web. Se desideri rimuovere i certificati SSL, [contatta il supporto](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* Se il dominio che aggiungi è elencato come qualsiasi cosa diversa da un CNAME, la possibilità di aggiungere ulteriori domini di tracciamento con brand sarà bloccata. Dovrai modificare qualsiasi dominio esistente e assicurarti che sia un record CNAME e non, ad esempio, un record A. Il pulsante Aggiungi verifica dinamicamente solo la presenza di CNAME e CNAME.

>[!MORELIKETHIS]
>
>[Modifica il dominio di branding predefinito](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
