---
description: Modelli e-mail per le vendite transazionali - Documenti Marketo - Documentazione del prodotto
title: Modelli e-mail per vendite transazionali
feature: Marketo Sales Connect
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# Modelli e-mail per vendite transazionali {#transactional-sales-email-templates}

Se il team invia e-mail transazionali o non commerciali, puoi contrassegnare un modello e-mail come non commerciale, in modo che possa ignorare gli annullamenti dell’iscrizione.

## Aspetti da considerare {#things-to-note}

* Le e-mail non commerciali ignoreranno gli annullamenti delle vendite e l&#39;assegno di annullamento dell&#39;abbonamento di [ Marketi Engage](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, ma non ignoreranno [domini bloccati](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md){target="_blank"}.

* I messaggi di annullamento dell&#39;iscrizione non verranno aggiunti automaticamente alle e-mail non commerciali, anche se l&#39;impostazione di amministrazione [aggiungi messaggi di annullamento dell&#39;iscrizione](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} è abilitata. Tuttavia, il `{{team_unsubscribe}}` [campo dinamico](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"} popolerà ancora il messaggio di annullamento dell&#39;iscrizione del team.

## Configurare un modello di e-mail per uso non commerciale {#configure-an-email-template-for-non-commercial-use}

1. Nell&#39;intestazione fare clic su **Modelli**.

   ![](assets/transactional-sales-email-templates-1.png)

1. Trova e seleziona il modello da aggiornare.

   ![](assets/transactional-sales-email-templates-2.png)

1. Abilita l’interruttore dell’e-mail non commerciale in Impostazioni modello.

   ![](assets/transactional-sales-email-templates-3.png)

## Invia un messaggio e-mail non commerciale {#send-a-non-commercial-email}

>[!NOTE]
>
>Quando viene selezionata una persona non iscritta, questa viene evidenziata in arancione.

1. Nell&#39;intestazione fare clic su **Componi**. Trova e seleziona il modello non commerciale desiderato.

   ![](assets/transactional-sales-email-templates-4.png)

1. Gli utenti visualizzeranno un banner che mostra loro di aver selezionato un modello e-mail non commerciale.

   ![](assets/transactional-sales-email-templates-5.png)

1. Fai clic su **Invia**.

   ![](assets/transactional-sales-email-templates-6.png)

L’e-mail verrà comunque inviata anche se la persona non è abbonata.
