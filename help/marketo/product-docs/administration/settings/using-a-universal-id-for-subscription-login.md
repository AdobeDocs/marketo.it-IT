---
unique-page-id: 10100311
description: Utilizzo di un ID universale per l’accesso all’abbonamento - Documenti Marketo - Documentazione del prodotto
title: Utilizzo di un ID universale per l’accesso all’abbonamento
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Utilizzo di un ID universale per l’accesso alla sottoscrizione {#using-a-universal-id-for-subscription-login}

Un ID universale consente di accedere a più abbonamenti Marketo con un singolo accesso e di passare rapidamente da un’iscrizione all’altra. Tuttavia, se lo desideri, puoi utilizzare diversi accessi per le tue iscrizioni.

Con l’ID universale, puoi comunque creare ticket di supporto per ciascuno dei tuoi abbonamenti individuali.

Le impostazioni a livello di iscrizione vengono rispettate per gli utenti che utilizzano l’ID universale, ad esempio ruoli, autorizzazioni e criteri per le password. Le modifiche a livello di profilo utente si riflettono in tutte le sottoscrizioni, ad esempio nome, cognome e indirizzo e-mail.

## Impostazione di un ID universale {#setting-up-a-universal-id}

Da ogni singola istanza, il tuo amministratore Marketo deve invitarti a ciascuno dei tuoi diversi abbonamenti con lo stesso accesso. Marketo non può unire automaticamente gli accessi esistenti. Dopo aver abilitato l&#39;ID universale, **l&#39;istanza Marketo non sarà disponibile** per un massimo di 30 minuti. Se hai una base di utenti più ampia, potrebbe essere un po&#39; più lunga.

>[!CAUTION]
>
>Se per un utente è abilitato un ID singolo o universale, i relativi ruoli e aree di lavoro possono **non** essere modificati dopo la configurazione iniziale.

>[!NOTE]
>
>Se disponi di più ID di accesso all’abbonamento, puoi avere anche più profili di community. Accertati di scegliere l’ID per l’ID universale connesso al profilo che desideri utilizzare, ovvero per l’istanza di produzione e non per la sandbox.

## Accesso {#logging-in}

Quando effettui l’accesso per accettare un invito per un secondo abbonamento utilizzando un ID universale, verrà visualizzata la pagina di accesso di Opt-in. In questo caso, devi selezionare una casella di controllo per accettare i termini e le condizioni. Dopo aver accettato, visualizzerai la pagina di ripristino normale, non questa, per tutti gli accessi successivi. Accettando i termini e le condizioni, consente a Marketo di distribuire i dati di profilo di base (come nome, cognome e indirizzo e-mail) ai centri dati in posizioni diverse in cui è ospitato l’abbonamento.

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>Gli ID che non utilizzi più rimangono a meno che l’amministratore della sottoscrizione li elimini. Ti consigliamo di conservarli, nel caso, ad esempio, in cui disponi di un rapporto privato, assegnato a te stesso, accessibile solo utilizzando tale ID. In questo caso, ha senso spostare questi rapporti privati nel nuovo ID universale e quindi eliminare l&#39;ID esistente.

## Password {#passwords}

Con l’ID universale per più abbonamenti, Marketo applica automaticamente i criteri di password più rigorosi. Ad esempio, se alcune sottoscrizioni richiedono una lunghezza minima della password e altre no, la lunghezza minima verrà applicata a tutte le sottoscrizioni.

Con un ID universale per più abbonamenti, puoi solo modificare la password.

>[!NOTE]
>
>Marketo chiederà agli utenti che desiderano utilizzare l’ID universale di reimpostare la password se la password dell’abbonamento corrente non è conforme ai criteri per le password del secondo abbonamento al quale sono invitati.

## Passaggio tra sottoscrizioni {#switching-between-subscriptions}

Utilizzando un ID universale, puoi visualizzare l’abbonamento a cui hai effettuato l’accesso e selezionare altre sottoscrizioni a cui hai accesso. Nella maggior parte dei casi, è possibile passare da una all’altra senza dover disconnettersi e accedere di nuovo.

![](assets/image2016-11-3-15-3a10-3a16.png)

Quando disconnetti e accedi di nuovo, Marketo effettua automaticamente l’accesso all’ultima sottoscrizione a cui sei stato effettuato l’accesso. Se necessario, puoi passare a un abbonamento diverso.

## Profili community {#community-profiles}

Se disponi di più abbonamenti, puoi avere più profili di community. È consigliabile scegliere l’accesso collegato al profilo community più attivo.

## Piattaforma mobile {#mobile-platform}

Gli utenti con ID universale possono visualizzare i propri dati su Marketo Moments e sull’applicazione di check-in degli eventi per iPad dall’abbonamento a cui hanno effettuato l’ultimo accesso. Non è possibile modificare gli abbonamenti dalla piattaforma Mobile stessa.

>[!MORELIKETHIS]
>
>* [Aggiungere Single Sign-On a un portale](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Limita accesso utente solo a SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [Invitare gli utenti Marketo a due istanze con ID universale](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

