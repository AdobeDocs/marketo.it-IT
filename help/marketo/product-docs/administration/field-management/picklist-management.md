---
description: Inserire qui la descrizione.
title: Gestione elenchi a discesa
hide: true
hidefromtoc: true
feature: Field Management
source-git-commit: 3c9facaed46a72c12a8a604aa9d22b47e28183cb
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Gestione elenchi a discesa {#picklist-management}

La gestione degli elenchi di selezione consente di definire un set fisso di valori per un campo al fine di semplificare la gestione dei dati e dei flussi di lavoro in Marketo Engage. Solo i campi non di testo non mappati a un campo CRM con un elenco a discesa definito possono essere gestiti in Marketo. Se un campo è mappato a un campo CRM che ha un elenco di selezione definito, i valori per tale campo devono essere definiti nel CRM.

È possibile visualizzare lo stato di un elenco a discesa dalla relativa pagina Gestione campi. Un campo può avere uno dei seguenti stati dell’elenco a discesa:

* **Gestito**: un utente ha definito il set di valori che possono essere suggeriti automaticamente per questo campo. Solo i valori definiti nella gestione dei campi vengono suggeriti automaticamente. Se un elenco a discesa gestito viene eliminato, lo stato dell&#39;elenco torna al valore iniziale del campo, Non gestito o Predefinito.

* **Non gestito**: i valori possibili per questo campo non sono definiti. I valori vengono suggeriti automaticamente in base a quelli esistenti in tali campi nel database.

* **Predefinito**: il campo include un elenco di valori definito dal sistema suggeriti all&#39;utente.

* **CRM**: il campo include un valore definito dal sistema CRM, Salesforce.com o Microsoft Dynamics, che è sincronizzato con l&#39;istanza.

  ![](assets/picklist-management-1.png)

## Gestione elenco a discesa {#manage-picklist}

Per modificare i valori di un campo, passare a **Amministratore** > **Gestione campi** e selezionare il campo desiderato.

Fai clic sul menu a discesa _Azioni campo_ e seleziona **Gestisci elenco a discesa**.

![](assets/picklist-management-2.png)

Nella finestra di dialogo _Gestisci elenco a discesa_ puoi aggiungere, modificare o eliminare valori. Puoi anche eliminare l&#39;elenco di selezione gestito per ripristinare lo stato originale del campo, _Non gestito_ o _Predefinito_.

![](assets/picklist-management-3.png)

Ogni voce dell’elenco a discesa ha un valore visualizzato e un valore inviato. Il valore di visualizzazione è ciò che viene suggerito all’utente durante la creazione di elenchi avanzati, campagne avanzate o moduli, mentre il valore inviato è quello memorizzato. Ad esempio, il caso di utilizzo del Codice territorio potrebbe suggerire il nome completo di un territorio (ad esempio, Alberta), durante la memorizzazione del codice a due lettere (AB).

## Suggerimento automatico {#autosuggest}

### Passaggio tra elenchi di selezione gestiti e non gestiti {#switching}

La maggior parte degli abbonamenti a Marketo Engage contiene dati precedenti all’introduzione degli elenchi di scelta gestiti. Per utilizzare i valori negli elenchi avanzati o nei passaggi del flusso da questo elenco di selezione delle versioni non gestite (ad esempio, dall’intero set di valori esistenti nei record del database), attiva l’impostazione Elenco di selezione gestito nella vista Elenco avanzato o Campagna. Quando è attivata, vengono visualizzati solo i valori dell’elenco a discesa gestito. Quando viene disattivato, viene utilizzato l’elenco a discesa non gestito e i valori vengono suggeriti automaticamente in base ai valori esistenti nel database.

### Elenchi Di Selezione Moduli (Seleziona Campi Tipo) {#form-picklists}

Analogamente agli elenchi di selezione predefiniti e gestiti da CRM, i valori per gli elenchi di selezione gestiti si propagano in Forms quando si utilizza il tipo di campo Seleziona. Per un campo con un elenco a discesa gestito, selezionare tale campo e impostare Tipo campo su _Seleziona_.

![](assets/picklist-management-4.png)

Mostra il set di valori dell’elenco a discesa gestito definiti per quel campo.

![](assets/picklist-management-5.png)
