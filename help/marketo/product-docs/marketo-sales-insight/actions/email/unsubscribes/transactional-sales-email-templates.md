---
description: Modelli e-mail per le vendite transazionali - Documenti Marketo - Documentazione del prodotto
title: Modelli e-mail per vendite transazionali
hide: true
hidefromtoc: true
feature: Sales Insight Actions
source-git-commit: f11e455196cdfb7a6c1054df40344cab5b06772b
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# Modelli e-mail per vendite transazionali {#transactional-sales-email-templates}

Se il team invia e-mail transazionali o non commerciali, puoi contrassegnare un modello e-mail come non commerciale, in modo che possa ignorare gli annullamenti dell’iscrizione.

## Aspetti da considerare {#things-to-note}

* Le e-mail non commerciali ignoreranno gli annullamenti delle vendite e [Verifica annullamento iscrizione Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, but will not bypass [blocked domains](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}.

* I messaggi di annullamento dell’abbonamento non verranno aggiunti automaticamente alle e-mail non commerciali, anche se [aggiungi impostazione di amministrazione messaggi di annullamento iscrizione](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} is enabled. However, the `{{team_unsubscribe}}`[dynamic field](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} compilerà comunque il messaggio di annullamento dell’iscrizione del team.

## Configurare un modello di e-mail per uso non commerciale {#configure-an-email-template-for-non-commercial-use}

Passa alla sezione del modello.

Cercare il modello che si desidera aggiornare.

Seleziona il modello.

Abilita l’interruttore dell’e-mail non commerciale in Impostazioni modello.

Inviare un’e-mail non commerciale

Quando viene selezionata una persona non iscritta, questa viene evidenziata in arancione.

Nella finestra di composizione selezionare il modello non commerciale che si desidera visualizzare.

Gli utenti visualizzeranno un banner che mostra loro di aver selezionato un modello e-mail non commerciale.

Fai clic su Invia; l’e-mail verrà comunque inviata anche se la persona non è più abbonata.
