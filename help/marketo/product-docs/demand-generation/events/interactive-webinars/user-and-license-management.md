---
description: Gestione di utenti e licenze - Documentazione di Marketo - Documentazione del prodotto
title: Gestione di utenti e licenze
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
feature: Interactive Webinars
source-git-commit: 0ab3b8075923f58a9546acff8039d67126f22bf3
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Gestione di utenti e licenze {#user-and-license-management}

Scopri come aggiungere e rimuovere utenti e visualizzare le licenze correnti.

## Aggiungi un utente {#add-a-user}

1. Vai all&#39;area **Amministratore**.

   ![](assets/user-and-license-management-1.png)

1. Fai clic su **Webinar interattivi**.

   ![](assets/user-and-license-management-2.png)

1. Fare clic su **Aggiungi/Rimuovi utenti**.

   ![](assets/user-and-license-management-3.png)

1. Fare clic sul menu a discesa Utenti disponibili, selezionare gli utenti che si desidera aggiungere e fare clic su **OK**.

   ![](assets/user-and-license-management-4.png)

## Rimuovi un utente {#remove-a-user}

1. Vai all&#39;area **Amministratore**.

   ![](assets/user-and-license-management-5.png)

1. Fai clic su **Webinar interattivi**.

   ![](assets/user-and-license-management-6.png)

1. Fare clic su **Aggiungi/Rimuovi utenti**.

   ![](assets/user-and-license-management-7.png)

1. Evidenziare gli utenti che si desidera rimuovere e premere il tasto Canc sulla tastiera. Al termine, fai clic su **OK**.

   ![](assets/user-and-license-management-8.png)

## Utilizzo delle licenze {#license-usage}

I webinar interattivi offrono licenze specifiche per la creazione di eventi basati su Adobe Connect. Ogni volta che viene aggiunta una licenza, viene visualizzata una nuova casella di utilizzo della licenza. Gli amministratori di Marketo possono visualizzare (non modificare) le licenze seguendo la procedura riportata di seguito. Contatta l’Adobe Account Team (il tuo Account Manager) per ottenere ulteriori licenze.

1. Vai all&#39;area **Amministratore**.

   ![](assets/user-and-license-management-9.png)

1. Fai clic su **Webinar interattivi**.

   ![](assets/user-and-license-management-10.png)

1. Scorri verso il basso fino alle schede Utilizzo licenze.

   ![](assets/user-and-license-management-11.png)

<table> 
  <tr>
   <td width="20%"><b>Data inizio</b></td>
   <td width="80%">Data di inizio della licenza.</td>
  </tr>
  <tr> 
   <td width="20%"><b>Data di scadenza</b></td>
   <td width="80%">Data di scadenza della licenza.</td>
  </tr>
  <tr> 
   <td width="20%"><b>Tipo</b></td>
   <td width="80%">Tipo di licenza acquistata. Sono disponibili tre tipi di licenza: Shared Events License, Shared Rooms License, Additional Storage License.</td>
  </tr>
  <tr> 
   <td width="20%"><b>Capacità evento</b></td>
   <td width="80%">Il numero massimo di partecipanti che possono essere ospitati in un evento.</td>
  </tr>
  <tr> 
   <td width="20%"><b>Eventi totali</b></td>
   <td width="80%">Numero totale di eventi per i quali è stato eseguito il provisioning con questa licenza.</td>
  </tr>
  <tr> 
   <td width="20%"><b>Eventi utilizzati</b></td>
   <td width="80%">Numero totale di eventi completati.</td>
  </tr>
  <tr> 
   <td width="20%"><b>Capacità di archiviazione</b></td>
   <td width="80%">Quantità di storage disponibile per l'archiviazione di registrazioni, materiale collaterale, heri images, documentazione e altre risorse.</td>
  </tr>
  </tbody>
</table>

**Aspetti da considerare**

* Il tipo &quot;Licenza di archiviazione aggiuntiva&quot; fornisce solo l&#39;archiviazione, pertanto il valore in ogni campo _oltre_ Capacità di archiviazione verrà elencato semplicemente come &quot;-&quot;.

* Il tipo &quot;Shared Room License&quot; ha eventi illimitati e &quot;Additional Storage License&quot; fornisce solo storage, pertanto il campo Total Events (Eventi totali) per queste licenze verrà elencato semplicemente come &quot;-&quot;.

* Ogni volta che un evento viene creato, verrà conteggiato come &quot;consumato&quot; dalla rispettiva licenza (a meno che non si tratti di una licenza per sala condivisa). La preferenza verrà data a &quot;Shared Event License&quot; se sono presenti sia &quot;Shared Event License&quot; che &quot;Shared Room License&quot; della stessa capacità. Se l&#39;evento non è stato consegnato e il programma eventi viene eliminato prima dell&#39;ora pianificata, il conteggio degli eventi viene rifornito sottraendo un evento dagli eventi consumati.

* Una volta esaurita la licenza, il riquadro rimane nella schermata Webinar interattivi della sezione Amministratore con &quot;Eventi totali&quot; e &quot;Eventi consumati&quot; che hanno lo stesso valore. La licenza verrà rimossa dalla schermata solo alla scadenza.

## Accesso utente {#user-access}

I webinar interattivi hanno la funzionalità di regolare l’utilizzo, consentendo agli utenti del Marketo Engage di creare e distribuire webinar interattivi. Tuttavia, un utente di un webinar interattivo (o non utente) potrebbe ancora avere accesso in lettura/modifica ai programmi di eventi di un webinar interattivo creati da altri utenti.

Gli utenti di Marketo che dispongono delle autorizzazioni per i webinar interattivi e sono proprietari di un particolare programma di eventi per webinar interattivi saranno in grado di eseguire tutte le funzioni del webinar interattivo relative a tale programma. Ciò include: creazione, accesso, modifica, clonazione, spostamento ed eliminazione del programma. Tuttavia, una volta che tale utente non è più un utente del webinar interattivo, il proprietario del programma sarebbe in grado di accedere al programma e spostarlo, ma non di eseguire altre funzioni.

Gli utenti di Marketo a cui sono state concesse le autorizzazioni per i webinar interattivi e che sono _non_ proprietari di un particolare programma di eventi per webinar interattivi potrebbero eseguire funzioni limitate su tali programmi. Gli utenti non amministratori di Marketo potranno accedere al programma e clonarlo, ma non potranno eseguire altre funzioni se dispongono delle autorizzazioni per i webinar interattivi. Tuttavia, gli utenti amministratori di Marketo _saranno_ in grado di eseguire tutte le funzioni, quali l&#39;accesso, la modifica, la clonazione, lo spostamento e l&#39;eliminazione di tale programma (purché dispongano delle autorizzazioni per i webinar interattivi). Una volta revocata questa autorizzazione per gli utenti amministratori e non amministratori di Marketo, questi potranno solo accedere al Programma di eventi del webinar interattivo e non potranno eseguire altre funzioni.

La limitazione delle funzioni utilizzabili è indicata da un pulsante di azione disattivato e da un messaggio al passaggio del mouse. Alcuni esempi dei pulsanti di azione disattivati sono &quot;Progettare il webinar&quot; o &quot;Immettere il webinar&quot;. Per le funzioni non utilizzabili, viene fornito un messaggio che evidenzia le restrizioni. Vedi l’esempio seguente:

![](assets/user-and-license-management-12.png)
