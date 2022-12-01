---
description: Modificare i limiti di recupero di oggetti personalizzati in Velocity Scripting - Marketo Docs - Documentazione del prodotto
title: Modificare i limiti di recupero oggetti personalizzati negli script Velocity
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
source-git-commit: aeaf1f55b81da70ac8415cab265165a3848b5a0e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Modificare i limiti di recupero oggetti personalizzati negli script Velocity {#change-custom-object-retrieval-limits-in-velocity-scripting}

Se utilizzi lo script Velocity per visualizzare i dati di oggetti personalizzati nelle e-mail, questa funzione potrebbe essere utile per te. Per impostazione predefinita, è possibile accedere a 10 oggetti personalizzati principali da Velocity Script. Se devi accedere a ulteriori informazioni, continua a leggere.

## Che cos’è Velocity {#what-is-velocity}

[Apache Velocity](https://velocity.apache.org/) è un linguaggio basato su Java progettato per la creazione di modelli e script di contenuti HTML. Marketo consente di utilizzarlo nel contesto delle e-mail tramite l’utilizzo di [token di scripting](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Ciò consente, tra l’altro, l’accesso ai dati archiviati negli oggetti personalizzati.

È possibile fare riferimento a oggetti personalizzati principali e secondari direttamente collegati al lead o al contatto, ma non a oggetti personalizzati di terzo livello. Per ogni oggetto personalizzato, i 10 record aggiornati più di recente per persona/contatto sono disponibili in fase di runtime e vengono ordinati dall’ultimo aggiornamento (a 0) al più vecchio aggiornamento (a 9).

## Come modificare il limite {#how-to-change-the-limit}

1. Vai a **Amministratore** sezione .

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Fai clic su **E-mail**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. Nella tabella Limiti di recupero oggetti personalizzati, immetti un nuovo limite di recupero padre e fai clic su **Salva modifiche**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>Il valore del limite di recupero padre deve essere compreso tra 10 e 100. Il limite di recupero figlio viene impostato automaticamente. Questo viene fatto dividendo 1000 per il limite di recupero padre. Ad esempio, se si imposta il limite Padre su 50, il limite Figlio diventa 20 (1000 ÷ 50 = 20).

Dolce! Ora è possibile accedere a più oggetti personalizzati dallo script Velocity.
