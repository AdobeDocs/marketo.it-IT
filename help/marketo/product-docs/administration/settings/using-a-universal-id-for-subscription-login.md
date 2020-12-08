---
unique-page-id: 10100311
description: Utilizzo di un ID universale per l'accesso all'iscrizione - Documenti Marketo - Documentazione prodotto
title: Utilizzo di un ID universale per l’accesso all’iscrizione
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---


# Utilizzo di un ID universale per l’accesso all’iscrizione {#using-a-universal-id-for-subscription-login}

Un ID universale consente di accedere a più iscrizioni Marketo con un singolo login e di passare rapidamente da un’iscrizione all’altra. Tuttavia, potete utilizzare accessi diversi per le iscrizioni.

Con l&#39;ID universale, potete comunque creare biglietti di supporto per ciascuna delle vostre iscrizioni individuali.

Le impostazioni a livello di iscrizione vengono rispettate per gli utenti che utilizzano l&#39;ID universale, ad esempio ruoli, autorizzazioni e criteri per le password. Le modifiche a livello di profilo utente si riflettono in tutte le iscrizioni, ad esempio nome, cognome e indirizzo e-mail.

## Impostazione di un ID universale {#setting-up-a-universal-id}

Da ogni singola istanza, l’amministratore di Marketo deve invitarvi a ciascuna delle vostre diverse iscrizioni con lo stesso login. Marketo non può unire automaticamente i tuoi accessi esistenti. Una volta attivato l&#39;ID universale, **l&#39;istanza Marketo non sarà più disponibile** per un massimo di 30 minuti. Se si dispone di una base utente più ampia, potrebbe essere un po&#39; più lunga.

>[!CAUTION]
>
>Se per un utente è abilitato Single ID o Universal ID, i ruoli e le aree di lavoro di tale utente **non** possono essere modificati dopo la configurazione iniziale.

>[!NOTE]
>
>Se disponete di più ID di accesso per l&#39;iscrizione, potete anche avere più profili per la community. Accertatevi di scegliere l’ID per l’ID universale collegato al profilo che desiderate utilizzare, vale a dire per l’istanza di produzione e non per la sandbox.

## Accesso {#logging-in}

Quando accedete per accettare un invito a un secondo abbonamento utilizzando un ID universale, viene visualizzata la pagina di accesso per il consenso. Qui è necessario selezionare una casella di controllo per accettare i termini e le condizioni. Una volta accettato, verrà visualizzata la pagina di ripristino normale, non questa, per tutti gli accessi successivi. Accettando i termini e le condizioni, potete consentire a Markeche di distribuire i dati di base del profilo (ad esempio nome, cognome e indirizzo e-mail) ai datacenter in diverse ubicazioni in cui si trova l&#39;iscrizione.

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>Gli ID che non utilizzate rimangono invariati a meno che l&#39;amministratore di iscrizione li elimini. Vi consigliamo di tenerli, nel caso, ad esempio, in cui disponiate di un rapporto privato, a cui potete accedere solo utilizzando tale ID. In questo caso, ha senso spostare questi rapporti privati nel nuovo ID universale, quindi eliminare l&#39;ID esistente.

## Password {#passwords}

Con l&#39;ID universale per più iscrizioni, Marketo applica automaticamente i criteri per le password più severi. Ad esempio, se alcune iscrizioni richiedono una lunghezza minima della password e altre no, la lunghezza minima sarà applicata a tutte le sottoscrizioni.

Con un ID universale per più iscrizioni, è possibile modificare solo la password.

>[!NOTE]
>
>Marketo chiederà agli utenti che desiderano utilizzare l’ID universale di reimpostare la password se la password dell’iscrizione corrente non è conforme ai criteri per la password del secondo abbonamento al quale sono invitati.

## Passaggio tra iscrizioni {#switching-between-subscriptions}

Utilizzando un ID universale, potete visualizzare l’iscrizione a cui avete effettuato l’accesso e selezionare altre iscrizioni a cui avete accesso. Nella maggior parte dei casi, è possibile passare da una all&#39;altra senza dover disconnettersi e rientrare.

![](assets/image2016-11-3-15-3a10-3a16.png)

Quando disconnetti e accedi di nuovo, Marketo ti connette automaticamente all&#39;abbonamento a cui hai effettuato l&#39;ultimo accesso. Se necessario, potete passare a un’altra iscrizione.

## Profili community {#community-profiles}

Se disponete di più iscrizioni, potete disporre di più profili di community. È consigliabile scegliere il login collegato al profilo community più attivo.

## Piattaforma mobile {#mobile-platform}

Gli utenti con ID universale possono visualizzare i propri dati sui Momenti di Marketo e sull’applicazione di check-in evento per l’iPad dall’ultima iscrizione a cui hanno effettuato l’accesso. Non è possibile modificare le iscrizioni dalla piattaforma Mobile stessa.

