---
description: Modelli e-mail per le vendite transazionali - Documenti Marketo - Documentazione del prodotto
title: Modelli e-mail per vendite transazionali
hide: true
hidefromtoc: true
feature: Marketo Sales Connect
source-git-commit: d6a3d95ed42d1c08d69014e1aa013e7436bd06c2
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Modelli e-mail per vendite transazionali {#transactional-sales-email-templates}

Se il team invia e-mail transazionali o non commerciali, puoi contrassegnare un modello e-mail come non commerciale, in modo che possa ignorare gli annullamenti dell’iscrizione.

## Aspetti da considerare {#things-to-note}

* Le e-mail non commerciali ignoreranno gli annullamenti delle vendite e [Verifica annullamento iscrizione Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, but will not bypass [blocked domains](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}.

* I messaggi di annullamento dell’abbonamento non verranno aggiunti automaticamente alle e-mail non commerciali, anche se [aggiungi impostazione di amministrazione messaggi di annullamento iscrizione](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} is enabled. However, the `{{team_unsubscribe}}` [dynamic field](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} compilerà comunque il messaggio di annullamento dell’iscrizione del team.

## Configurare un modello di e-mail per uso non commerciale {#configure-an-email-template-for-non-commercial-use}

1. Nell’intestazione, fai clic su **Modelli**.

PICC

1. Cercare il modello che si desidera aggiornare.

PICC

1. Seleziona il modello.

PICC

1. Abilita l’interruttore dell’e-mail non commerciale in Impostazioni modello.

PICC

## Invia un messaggio e-mail non commerciale {#send-a-non-commercial-email}

Quando viene selezionata una persona non iscritta, questa viene evidenziata in arancione.

1. Nella finestra di composizione selezionare il modello non commerciale che si desidera visualizzare.

PICC

1. Gli utenti visualizzeranno un banner che mostra loro di aver selezionato un modello e-mail non commerciale.

PICC

1. Clic **Invia**.

PICC

L’e-mail verrà comunque inviata anche se la persona non è abbonata.
