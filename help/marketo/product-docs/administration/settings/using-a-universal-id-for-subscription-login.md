---
unique-page-id: 10100311
description: Utilizzo di un ID universale per l’accesso in abbonamento - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo di un ID universale per l’accesso in abbonamento
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
feature: Administration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Utilizzo di un ID universale per l’accesso in abbonamento {#using-a-universal-id-for-subscription-login}

Un Universal ID consente di accedere a più abbonamenti Marketo con un singolo accesso e di passare rapidamente da un abbonamento all’altro. Tuttavia, se lo desideri, puoi utilizzare diversi accessi per i tuoi abbonamenti.

Con Universal ID, puoi comunque creare i ticket di supporto per ciascuno dei tuoi abbonamenti.

Le impostazioni del livello di abbonamento vengono rispettate per gli utenti che utilizzano l’ID universale, ad esempio ruoli, autorizzazioni e criteri per le password. Le modifiche al livello di profilo utente si riflettono in tutte le sottoscrizioni, ad esempio nome, cognome e indirizzo e-mail.

## Impostazione di un ID universale {#setting-up-a-universal-id}

Tutti gli abbonamenti Marketo sono forniti con la funzione Universal ID opzionale. Da ogni singola istanza, il tuo amministratore di Marketo deve invitarti a ciascuno dei tuoi abbonamenti diversi con lo stesso accesso. Marketo non può unire automaticamente gli accessi esistenti.

>[!NOTE]
>
>Se disponi di più ID di accesso per abbonamento, puoi anche disporre di più profili community. Assicurati di scegliere l’ID del tuo Universal ID connesso al profilo che desideri utilizzare e che sia per la tua istanza di produzione, non per la sandbox.

## Accesso {#logging-in}

Quando accedi per accettare un invito a un secondo abbonamento utilizzando un ID universale, viene visualizzata la pagina di accesso di Opt-in. In questo caso, seleziona una casella di controllo per accettare i termini e le condizioni. Dopo aver accettato, verrà visualizzata la normale pagina di reimpostazione, non questa, per gli accessi successivi. Accettando i termini e le condizioni, Marketo consente di distribuire i dati di profilo di base (come nome, cognome e indirizzo e-mail) ai centri dati in posizioni diverse in cui è ospitato l’abbonamento.

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>Gli ID che non utilizzi più rimangono invariati a meno che l’amministratore della sottoscrizione non li elimini. È consigliabile conservarli, ad esempio nel caso in cui si disponga di un rapporto privato, assegnato a se stessi, a cui è possibile accedere solo utilizzando tale ID. In questo caso, ha senso spostare questi rapporti privati nel nuovo ID universale e quindi eliminare l’ID esistente.

## Password {#passwords}

Con l’ID universale per più abbonamenti, Marketo applica automaticamente i criteri per la password più rigorosi. Ad esempio, se alcuni abbonamenti richiedono una lunghezza minima della password e altri no, la lunghezza minima verrà applicata a tutti gli abbonamenti.

Con un ID universale per più abbonamenti, solo tu puoi modificare la password.

>[!NOTE]
>
>Marketo chiederà agli utenti che desiderano usare un Universal ID di reimpostare la propria password se la password dell’abbonamento corrente non è conforme ai criteri della password del secondo abbonamento a cui vengono invitati.

## Passaggio tra le sottoscrizioni {#switching-between-subscriptions}

Utilizzando un ID universale, puoi visualizzare l’abbonamento a cui hai effettuato l’accesso e selezionare altri abbonamenti a cui hai accesso. Nella maggior parte dei casi, è possibile passare da una all’altra senza dover disconnettersi ed effettuare nuovamente l’accesso.

![](assets/image2016-11-3-15-3a10-3a16.png)

Quando esci e accedi di nuovo, Marketo ti accede automaticamente all’ultimo abbonamento a cui hai effettuato l’accesso. Se necessario, puoi quindi passare a un abbonamento diverso.

## Profili community {#community-profiles}

Se disponi di più abbonamenti, puoi avere più profili community. È consigliabile scegliere l&#39;account di accesso collegato al profilo community più attivo.

## Piattaforma mobile {#mobile-platform}

Gli utenti con ID universale possono visualizzare i propri dati in Marketo Moments e nell’applicazione di archiviazione degli eventi di iPad dall’ultimo abbonamento a cui hanno effettuato l’accesso. Non è possibile modificare gli abbonamenti dalla piattaforma Mobile stessa.

>[!MORELIKETHIS]
>
>* [Aggiungere il Single Sign-On a un portale](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Limita l&#39;accesso degli utenti solo all&#39;SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [Invito degli utenti di Marketo a due istanze con ID universale](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
