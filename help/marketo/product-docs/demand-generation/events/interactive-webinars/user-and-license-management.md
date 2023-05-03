---
description: Gestione di utenti e licenze - Documenti Marketo - Documentazione del prodotto
title: Gestione di utenti e licenze
hide: true
hidefromtoc: true
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
source-git-commit: 9c3ec23cbd0a89f51cab40a51d76b4205baf9944
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Gestione di utenti e licenze {#user-and-license-management}

Scopri come aggiungere e rimuovere utenti e visualizzare le licenze correnti.

## Aggiungi un utente {#add-a-user}

1. Vai a **Amministratore** area.

   ![](assets/user-and-license-management-1.png)

1. Fai clic su **Webinar interattivi**.

   ![](assets/user-and-license-management-2.png)

1. Fai clic su **Aggiungi/rimuovi utenti**.

   ![](assets/user-and-license-management-3.png)

1. Fai clic sul menu a discesa Utenti disponibili, seleziona gli utenti da aggiungere e fai clic su **OK**.

   ![](assets/user-and-license-management-4.png)

## Rimuovere un utente {#remove-a-user}

1. Vai a **Amministratore** area.

   ![](assets/user-and-license-management-5.png)

1. Fai clic su **Webinar interattivi**.

   ![](assets/user-and-license-management-6.png)

1. Fai clic su **Aggiungi/rimuovi utenti**.

   ![](assets/user-and-license-management-7.png)

1. Evidenziare gli utenti da rimuovere e premere il tasto Canc sulla tastiera. Fai clic su **OK** al termine.

   ![](assets/user-and-license-management-8.png)

## Utilizzo della licenza {#license-usage}

I webinar interattivi offrono licenze specifiche per la creazione di eventi Adobe Connect. Ogni volta che viene aggiunta una licenza, viene visualizzata una nuova casella di utilizzo della licenza. Gli amministratori di Marketo possono visualizzare (non modificare) le licenze seguendo i passaggi seguenti. Contatta il team dell&#39;account Adobe (il tuo Account Manager) per acquisire licenze aggiuntive.

1. Vai a **Amministratore** area.

   ![](assets/user-and-license-management-9.png)

1. Fai clic su **Webinar interattivi**.

   ![](assets/user-and-license-management-10.png)

1. Scorri verso il basso fino alle schede Utilizzo licenza.

   ![](assets/user-and-license-management-11.png)

<table> 
  <tr> 
   <td><b>Data di inizio</b></td>
   <td>Data di inizio della licenza.</td>
  </tr>
  <tr> 
   <td><b>Data di scadenza</b></td>
   <td>Data di scadenza della licenza.</td>
  </tr>
  <tr> 
   <td><b>Tipo</b></td>
   <td>Tipo di licenza acquistata. Sono disponibili tre tipi: Licenza Eventi Condivisi, Licenza Stanze Condivise, Licenza Di Archiviazione Aggiuntiva.</td>
  </tr>
  <tr> 
   <td><b>Capacità evento</b></td>
   <td>Il numero massimo di partecipanti che possono essere inclusi in un evento.</td>
  </tr>
  <tr> 
   <td><b>Totale eventi</b></td>
   <td>Numero totale di eventi per i quali è stato eseguito il provisioning con questa licenza.</td>
  </tr>
  <tr> 
   <td><b>Eventi utilizzati</b></td>
   <td>Numero totale di eventi completati.</td>
  </tr>
  <tr> 
   <td><b>Capacità di storage</b></td>
   <td>Quantità di spazio di archiviazione disponibile per l'archiviazione di registrazioni, garanzie reali, heri images, documentazione e altre risorse.</td>
  </tr>
  </tbody>
</table>

**Aspetti da considerare**

* Il tipo &quot;Licenza di archiviazione aggiuntiva&quot; fornisce semplicemente lo storage, quindi il valore in ogni campo _inoltre_ La capacità di storage sarà indicata semplicemente come &quot;-&quot;.

* Il tipo &quot;Shared Room License&quot; ha eventi illimitati e &quot;Additional Storage License&quot; fornisce semplicemente spazio di archiviazione, pertanto il campo Total Events per queste licenze verrà elencato semplicemente come &quot;-&quot;.

* Ogni volta che un evento viene creato, viene conteggiato come &quot;consumato&quot; dalla rispettiva licenza (a meno che non si tratti di una Licenza di Stanza Condivisa). La preferenza verrà data a &quot;Licenza evento condivisa&quot; se sono presenti sia &quot;Licenza evento condiviso&quot; che &quot;Licenza stanza condivisa&quot; della stessa capacità. Se l’evento non è stato consegnato e il programma Evento viene eliminato prima dell’ora pianificata, il conteggio degli eventi viene ricompilato sottraendo un evento dagli eventi utilizzati.

* Una volta esaurita la licenza, la relativa porzione rimane nella schermata Webinar interattivi nella sezione Amministratore con &quot;Eventi totali&quot; e &quot;Eventi consumati&quot; con lo stesso valore. Solo alla scadenza della licenza verrà rimossa dalla schermata.
